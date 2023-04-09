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
