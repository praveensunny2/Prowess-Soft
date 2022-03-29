# Prowess-Soft
A Digital Internship on Java Full Stack Developer

> As part of Java Full Stack Developer, a 7 to 8 weeks training offered by ***Prowess Soft***, my week-wise learnings are as shown below :

## Unit I
TASK 1:

> Create a thread using Thread class and print the thread name

```ruby
class create extends Thread
{
    public void run()
    {
        System.out.println("<Thread Created> : "+ Thread.currentThread().getName() +  " By extending thread class");
    }
}
public class Main
{
    public static void main(String[] args)
    {
        create obj = new create();
        obj.start();
        
    }
}
```
