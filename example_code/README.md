## layout
```
<androidx.camera.view.PreviewView
        android:id="@+id/viewFinder"
        android:layout_width="350dp"
        android:layout_height="250dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.3"
        tools:layout_editor_absoluteX="-42dp" />

    <TextView
        android:id="@+id/messageView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="10dp"
        android:text="카메라를 정면으로 바라보세요."
        android:textSize="24sp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@id/viewFinder" />
```

## Activity
```Kotlin
class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        val binding = ActivityMainBinding.inflate(layoutInflater)
        val lib : FaceRecognitionLibrary
        class myClass : FaceRecognitionLibrary(this,this,5){
            override fun reachSeletedCount(vector: DoubleArray) {
              //you can use vector parameter
            }

        }
        val myLib=myClass()
        myLib.settingModule(this,this)
        myLib.startCamera(this,this,binding.viewFinder.surfaceProvider,binding.messageView)
        setContentView(binding.root)
    }
}
```
