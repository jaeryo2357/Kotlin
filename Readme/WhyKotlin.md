1.Why Kotlin
-------------

* **Kotlin**�� 2017�� 5�� ���ۿ��� �������� ������ �ȵ���̵� ����Դϴ�. Java�� ���� **���� ���α׷��� ���**�� JVM, Android, Browser, Native �ۿ� ���� �� �ֽ��ϴ�.

* **����**

  * **���Ἲ**
    * Kotlin�� ���� ū ������ �ϳ��� �ڵ��� ���� ���� ���Դϴ�.
      * JAVA
        <pre>
        class data{
        String name;
        String email;
        String company;
        
        String GetName(){
           return name;
        }
        void SetName(String name)
        {
          this.name=name;
        }
        
        ... ��� ��� ������ �ش��ϴ� Getter,Setter,equals(),hashCode(),toString(),copy() �� �����ؾ���
        
        </pre>
        
      * Kotlin
        <pre>
        data class Customer(val name: String, val email: String, val company: String)
        </pre>
  * **������**
  
    * Exception�� �߻��� **�ּ�ȭ**
    
      * Kotlin�� **NullPointException �ּ�ȭ**
        <pre>
        var output: String
        output=null // ������ ���� --> null ���� ���� �� ���� ������ ������ �߻���Ŵ
        </pre>
        <pre>
         val name: String? =null // Nullable Type
         println(name.lenght())  // ������ ���� �߻�--> null ���̸� ������ ����
        </pre>
        
        
        
     * �ڵ����� **Casting**
     
     
        * **Java**
          <pre>
           public void Func(Object obj)
           {
              if(obj instanceof Invoice)
                ((Invoice)obj).calcualteTotal();
           }
          </pre>
     
     
        * **Kotlin**
          <pre>
          fun Func(obj : Any) // Any�� java���� Object�� ���� �ֻ��� Ŭ����
          {
            if(obj is Invoice)
              obj.calculateTotal()
          }
          </pre>
          
          **Kotlin**�� if(obj is Invoice)���� obj�� **�ڵ����� Invoice�� Casting ��**
         
        






