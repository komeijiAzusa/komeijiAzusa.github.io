`package packageclass.test2;

public class message {
    private  String UserName;
    private int age;
    private String gender;

    public void setUserName(String name) {
        UserName = name;
    }

    public String getUserName() {
        return UserName;
    }

    public void setAge(int a) {
        if (a>0&&a<100)
        {
            age=a;
        }
        else {
            System.out.println("输入错误");
        }

    }

    public int getAge() {
        return age;
    }

    public void setGender(String sex) {
        gender = sex;
    }

    public String getGender() {
        return gender;
    }
}
`
`package packageclass.test2;

public class MessageTest {
    public static void main(String[] args)
    {
     message user1=new message();
     user1.setUserName("张三");
     user1.setAge(20);
     user1.setGender("男");
        System.out.println(user1.getUserName());
        System.out.println(user1.getAge());
        System.out.println(user1.getGender());

    }
}
`




