# HW2
public class Main {

	public static void main(String[] args) {
		
		System.out.println("Stack Test---");
		Stack testStack = new Stack(10);
		testStack.push(10);
		testStack.push(20);
		testStack.push(30);
		System.out.println("stack top:" + testStack.get_top());
		testStack.push(40);
		testStack.push(50);
		testStack.pop();
		testStack.push(30);
		System.out.println("print stack content:");
		testStack.print();
		System.out.println("print stack while it's not empty:");
		while (!testStack.is_empty()) {
			System.out.println(testStack.pop());
		}
			
		System.out.println("Queue Test---");
		Queue testQueue = new Queue();
		testQueue.enqueue(1);
		testQueue.enqueue(2);
		testQueue.enqueue(3);
		testQueue.enqueue(4);
		testQueue.enqueue(5);
		System.out.println("print queue content:");
		testQueue.print();
		testQueue.dequeue();
		System.out.println("print queue content after dequeue:");
		testQueue.print();		

	}
}
