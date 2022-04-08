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

> Create a thread using Runnable Interface and print the thread name

```ruby
class create implements Runnable
{
    public void run()
    {
        System.out.println("^Thread Created^: "+ Thread.currentThread().getName());
    }
}
public class Main
{
    public static void main(String args[])
    {
        create ob = new create();
        Thread th = new Thread(ob);
        th.start();
    }
}
```

TASK 2:

> Create 5 threads and print "Hello All" using Thread class

```ruby
class createthread extends Thread
{
    public void run()
    {
        System.out.println(Thread.currentThread().getName() + " Hello All");
    }
}
public class Main
{
    public static void main(String args[])
    {
        createthread ob1 = new createthread();
        createthread ob2 = new createthread();
        createthread ob3 = new createthread();
        createthread ob4 = new createthread();
        createthread ob5 = new createthread();
        ob1.start();
        ob2.start();
        ob3.start();
        ob4.start();
        ob5.start();

    }
}
```

> Create 5 threads and print "Hello India" using Thread Runnable Interface

```ruby
class create implements Runnable
{
    public void run()
    {
        System.out.println(Thread.currentThread().getName()+" Hello India");
    }
}
public class Main
{
    public static void main(String args[])
    {
        create ob1 = new create();
        Thread th1 = new Thread(ob1);
        th1.start();
        create ob2 = new create();
        Thread th2 = new Thread(ob2);
        th2.start();
        create ob3 = new create();
        Thread th3 = new Thread(ob3);
        th3.start();
        create ob4 = new create();
        Thread th4 = new Thread(ob4);
        th4.start();
        create ob5 = new create();
        Thread th5 = new Thread(ob5);
        th5.start();
        
    }
}
```

> Program on Executor Framework

```
Updating ...
```

TASK 3:

> To store group of integers using ArrayList

```ruby
import java.util.*;
class displayInt
{
	public static void main (String[] args)
	{
		ArrayList al = new ArrayList();
		for(int i = 11 ; i <= 20; i++)
		{
			al.add(i);
		}
		Iterator it = al.iterator();
		while(it.hasNext())
		{
			System.out.println(it.next());
		}
	}
}
```

> A Program using Queue Interface

```ruby
import java.util.*;
class Main
{
	public static void main (String[] args)
	{
		PriorityQueue pq = new PriorityQueue();

		for(int i=1;i<=6;i++)
		{
			pq.add(i);
		}

		Iterator it = pq.iterator();
		while(it.hasNext())
		{
			System.out.println(it.next());
		}
		//Deletes the front of the queue
		System.out.println("Dequeue element: "+pq.remove());	
		System.out.println("Dequeue element: "+pq.poll());
		
		Iterator it1 = pq.iterator();
		while(it1.hasNext())
		{
			System.out.println(it1.next());
		}
	}
}
```
> A Program using Stack Interface

```ruby
import java.util.*;
class Main
{
	public static void main (String[] args)
	{
		
		Stack st = new Stack();
		for(int i=10;i<=60;i=i+10)
		{
			st.push(i);
		}
		Iterator it = st.iterator();
		while(it.hasNext())
		{
			System.out.println(it.next());
		}
		
		System.out.println("Removed element: "+st.pop());
		System.out.println("Removed element: "+st.pop());
		
		Iterator it1 = st.iterator();
		while(it1.hasNext())
		{
			System.out.println(it1.next());
		}
	}
}
```
