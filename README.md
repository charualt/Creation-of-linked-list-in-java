# Creation-of-linked-list-in-java
There is a creation of linked list in java.

public class Demo {
Node head;//head of list
//making a node
 static class Node{
	int data;
	Node next;
	Node(int d)
	{
		data=d;
		next=null;
	}
 }
 //printing a node
	public  void printlist()
	{
		Node n=head;
		while(n!=null)
		{
			System.out.println(n.data+" ");
			n=n.next;
		}
	}
  public static void main(String[] args) {
	Demo ll=new Demo();
  ll.head=new Node(1);
	Node second=new Node(2);
	Node third=new Node(3);
	ll.head.next=second;
 second.next=third;
	ll.printlist();
