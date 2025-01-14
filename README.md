# Android-A-1
My Android codes-1
#Linear Activity
class LinearActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        enableEdgeToEdge()
        setContentView(R.layout.linear)
        var name=findViewById<EditText>(R.id.edittext1)
        var phone=findViewById<EditText>(R.id.edittext2)
        var b= findViewById<Button>(R.id.button1)
        var display=findViewById<TextView>(R.id.textView)
        b.setOnClickListener {
            var a=name.text.toString()
            var b=phone.text.toString()
            display.text="MY NAME IS " + a +" "+"PHONE IS"+  b

        }
    }
}
