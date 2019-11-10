* Loops
  ```scala
  for( i <- 1 to 10)
    println(i)
    
  //multiple variables
  for( i <- 1 to 5; j <- 6 to 10) {
    println(i)
    println(j)
  }
  //for each i it will print 6 to 10
  ```
* There is no `break` and `continue`
* Reading input:
  ```scala
  import scala.io.StdIn.{readLing, ...}
  readLine()  //read input as string
  readInt()
  readLong()
  readDouble()
  readByte()
  readShort()
  ```
* Printing output:
  ```scala 
  printf("Hello number: %d\n", 123)
  println(s"Hello world")
  
  val age = 90
  println(f"I am ${currentAge+2} years old")
  ```
* String manipulation:
  ```scala
  //indexing
  var arrString = "I am a string"
  println("3rd index element: " + arrString(3))
  
  //concatenation
  s1 = s1.concat(" end")
  
  //eqality
  s1.equals(s2) //returns boolean

  //get index of query string
  i = s1.indexOf("end")
  ```
* Functions:
  ```scala
  def foo(param1:<data type>, ...) : <return type> = {
    return param1 + param2  //return keyword not required
  }
  
  //functions which don't return => procedures
  def bar() : Unit = {
    <body>
  }
  ```
* Arrays:
  ```scala
  val arr = Array("hello", "world")
  arr(0) = "bye"  //modify 0th index. TODO: how val array is mutable?
  
  val arr = new Array[Int](10)  //array of 20 integers allocated
