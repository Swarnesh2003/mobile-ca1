 Var xx=  findviewbyid<type>(R.id.id of that widge)

Var name = xx.text.toString()

Var num = xx.text.toString().toInt()

xx.setText(name)

xx.onclicklisteniner(){

}

Spinner:
xx.selectedItem.toString()
xx.isChecked()




button.setOnClickListener() {  
            intent = Intent(this, SecondActivity::class.java)  
            intent.putExtra("id_value", id)  
            intent.putExtra("language_value", language)  
            startActivity(intent)  
  }  


class SecondActivity : AppCompatActivity() {


   override fun onCreate(savedInstanceState: Bundle?) {
       super.onCreate(savedInstanceState)
       setContentView(R.layout.activity_second)
       val data:TextView = findViewById(R.id.textView6 )
       var fs1 = intent.getStringExtra("Firstname")
       var ls1= intent.getStringExtra("Lastname")
      data.setText(fs1)


   }
}









