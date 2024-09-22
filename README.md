# Tower-of-hanoi
# In this we shift some disk of different size to another pole without changing their order

# first we make recursion class
public class Recursion2 {
# after we give parameters we use n is for no. of disk , helper is use for store disk for temporary and dest is the last stop or pole of disk. 
public static void tower0fHanoi(int n, String src, String helper, String dest) {

if (n == 1) {
System.out.println("transfer disk "+n+" from "+src+" to "+dest);
return;
}

towerOfHanoi(n-1, src, dest, helper);
System.out.println("transfer disk "+n+" from "+src+" to "+dest);
}

towerOfHanoi(n-1, helper, src, dest);


public static void main(String args[]) {

int n =3;
tower0fHanoi (n,"5","H","D");
 }

}
