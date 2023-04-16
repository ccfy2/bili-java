# bili-java
public class Main {
    public static void main(String[] args){
        //创建对象 容器
        StringBuilder sb = new StringBuilder();
        //链式添加字符串
        sb.append("aaa").append("bbb").append("ccc");
        System.out.println(sb);
        //变回字符串
        String str = sb.toString();
        System.out.println(str);
    }
}



public class Main {
    public static void main(String[] args){
      int[] arr = {1, 2, 3};
String str = arrToString(arr);
System.out.println(str);
    }
public static String arrToString(int[] arr){
        StringBuilder sb = new StringBuilder();
        sb.append("[");
        for(int i=0; i< arr.length ;i++){
            if(i==arr.length-1){
                sb.append(arr[i]);
            }else {
                sb.append(arr[i]).append(", ");
            }
        }
        sb.append("]");
        return sb.toString();
}
}



import java.util.ArrayList;

public class Main {
    public static void main(String[] args) {
       ArrayList<Student> list = new ArrayList<>();
       Student s1 = new Student("zhangsan", 23);
       Student s2 = new Student("lisi", 24);
        Student s3 = new Student("wangwu", 25);
        list.add(s1);
        list.add(s2);
        list.add(s3);
        for (int i = 0; i <list.size(); i++) {
            Student stu = list.get(i);
            System.out.println(stu.getName()+","+stu.getAge());

        }
    }
}

public class Student {
   private String name;
   private int age;

    public Student() {
    }

    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }

}

