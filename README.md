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



