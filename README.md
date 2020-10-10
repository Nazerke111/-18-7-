# -18-7-
Назерке Шадиева 
package naz.lab.pkg4;
public class NazLab4 {
    public static void main(String[] args) {
       System.out.println("Main thread 0");
       TestThread Thread = new TestThread();
       Thread.start();
    }
    }
class TestThread extends Thread {
    @Override 
    public void run() {
        for( int i=0;i<=1000;i++){
            System.out.println(this.getName()+ " - "+i);
        }
    }
    
}
