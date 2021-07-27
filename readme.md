

fun main() {
    val diasSemana:MutableList<String> = mutableListOf("Lunes","Martes")
    val diasVacio:MutableList<String> = mutableListOf()
    
    println(diasSemana)
    println(diasVacio)
    
    diasSemana.forEach{
        diasVacio.add(it +":")
    }
    
    println(diasSemana)
    println(diasVacio)
    
    }

	

fun mutablelist()
{
    
    //Listas mutables pueden cambiar sus valores
	val diasSemana:MutableList<String> = mutableListOf("Lunes","Martes")
    
    diasSemana.add("Miercoles")
    diasSemana.add("Jueves")
    diasSemana.add("Viernes")
		    
    diasSemana.add(0,"Semana: ")
   
    //println(diasSemana.last())
    println(diasSemana)
    
    //filtrar en mutablelist
    val resultado = diasSemana.filter{it  == "Lunes"}
    println(resultado)
    
    
    //filtrar en mutablelist
    val resultado2 = diasSemana.filter{it[0] == 'M' || it[0] == 'm'}
    println(resultado2)
    
    
    
}


fun arraylist()
{
    val diasSemana = arrayOf("Lunes", "MArtes", "Miercoles", "jueeves")
    
    println(diasSemana[2])
    diasSemana.set(2,"Mierrrrcoles")
    println(diasSemana[2])  
    //println(queMesEs(12))
    diasSemana.forEach{
    println(it)
        
    if(it == "Jueves") println("por fin jueves")
}
   
}

fun queMesEs(mes:Int):String
{
   return when(mes)
    {
        in 1..6 -> "Primer semestre"
        in 7..12 -> "Segundo semestre"
        !in 1..12 -> "No es un mes valido"
        else -> "No es un mes valido"
     }
}

fun ifelsemetodo()
{
     var soyUnPerro:Boolean = true
    
    if(soyUnPerro) 
    {
        //soy un perro
        println("soy un perro")
    }else
    {
        //No hacer nada
        println("no soy perro")
    }
}


fun sumar(numeroFavorito:Int, edad:Int)
    {
        
        val resultado = numeroFavorito + edad
        
        println(resultado)
        
    }
    
fun restar()
{
   val numeroFavorito = 13
   val edad = 27
   println(numeroFavorito - edad)
}
