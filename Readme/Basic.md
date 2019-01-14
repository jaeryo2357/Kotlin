2.�⺻����
-------------

* [HOME](./README.md)

> �� �Խñ��� Java�� Kotlin�� ���ϸ� �����մϴ�.
* **Package ��Ģ**
  * Package ������ **�ҽ����� �� ����** ���� �ؾ� ��

  <hr>
  <pre>
  package hello

  fun main(args : Array<String>){ ... }
  </pre>

  * **Kotlin���� Package�� ���� �ҽ��ڵ尡 ��ġ�� Directory�� ��ġ�� �ʿ䰡 ����.**

* **�Լ� ����**

  * kotlin�� **fun**Ű���带 ����Ͽ� �Լ��� �����ϸ� ��ȯŸ���� �� �ڿ� �ɴϴ�.

  * �Ű������� **name: type**���� ���ǵǸ� **�Ű��������� ,�� ���е˴ϴ�.**
  * **Java**

  <pre>
  int sum(int a,int b){
  return a+b;
  }
  </pre>

  * **Kotlin**

  <pre>
  fun sum(a: Int,b: Int):Int{
  return a+b
  }
  </pre>

  * ��ȯ���� ������ Java-> void , Kotlin -> **Unit**
   * **Java**
   <hr>
    <pre>
      void PrintValue(){
      System.out.print("hello");
      }
    </pre>

   * **Kotlin**
   <hr>
    <pre>
     fun PrintValue():Unit{
      print("hello")
      }
    </pre>
    > Unit�� ������ �� �ֽ��ϴ�.
    
     <pre>
     fun PrintValue(){
      print("hello")
      }
    </pre>
 * **���� ����**
    * **val**

      * val java���� **final**�� �����մϴ�. (���)

      * **Kotlin**

      <pre>
      val a:int=2
      val b=2  // ���� ������ int���� ����
      val c:int
      c=3 //�ѹ��� �ʱ�ȭ ����
      </pre>
        * **Java**

        <pre>
        final int a=2;
        final int a; //complie error ������ �ʱ�ȭ �ؾ���
        </pre>
    * **var**
      * var�� �ڹ��� �Ϲݺ����� �����ϴ�.
      <pre>
      var x=2
      </pre>
  * **�ּ�**
    * Kotlin
      * Kotlin������ �ּ��� Java�� �����մϴ�. 
      <pre>
       //            �� �� �ּ�

       /*   */       �� �ּ�
       
       /*
        /*
                      ��ø���� �ּ� ���� �� �ִ�.        
        */
        */
      </pre>
      
   * **���ڿ�**
     * Java
     <pre>
      int a=2;
      String s=" string test "+a+" is good";
     </pre>

     * Kotlin
     <pre>
     var a=2
     val s=" string test $a is good"  //$ ǥ�÷� value ���԰���

     var s2="string ${s.replace("is","was")},but now is &a" // �Լ�ȣ�� �κе� {}���̿� ���԰���
     </pre>

   * **�Լ��� ����**
     * �Լ��� ������ �� �������� ������ ���, ������ �Ҽ� �ִ�.

     <pre>
     fun sum(a:Int,b: Int):Int{
       return a+b
       }
     </pre>

     <pre>
     fun sum(a:Int,b: Int)=a+b
     </pre>