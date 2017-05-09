```java

public class Main {

    String strPrint = "{is_yellow_vip=0, msg=, vip=0, nickname=★AFinalStone, figureurl_qq_1=http://q.qlogo.cn/qqapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/40, city=杭州, figureurl_1=http://qzapp.qlogo.cn/qzapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/50, gender=男, province=浙江, is_yellow_year_vip=0, yellow_vip_level=0, figureurl=http://qzapp.qlogo.cn/qzapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/30, figureurl_2=http://qzapp.qlogo.cn/qzapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/100, is_lost=0, figureurl_qq_2=http://q.qlogo.cn/qqapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/100, level=0, ret=0}";

    public static void main(String[] args) {
        HashMap<String, Object> hashMap = new HashMap<String, Object>();
        hashMap.put("is_yellow_vip", 0);
        hashMap.put("msg", "");
        hashMap.put("vip", 0);
        hashMap.put("nickname", "★AFinalStone");
        hashMap.put("figureurl_qq_1", "http://q.qlogo.cn/qqapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/40");
        hashMap.put("city", "杭州");
        hashMap.put("figureurl_1", "http://qzapp.qlogo.cn/qzapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/50");
        hashMap.put("gender", "男");
        hashMap.put("province", "浙江");
        hashMap.put("is_yellow_year_vip", 0);
        hashMap.put("yellow_vip_level", 0);
        hashMap.put("figureurl", "http://qzapp.qlogo.cn/qzapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/30");
        hashMap.put("figureurl_2", "http://qzapp.qlogo.cn/qzapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/100");
        hashMap.put("is_lost", 0);
        hashMap.put("figureurl_qq_2", "http://q.qlogo.cn/qqapp/1105787820/B5E3E2C5A57C482C4A1E0DF78C7E10D7/100");
        hashMap.put("level", 0);
        hashMap.put("ret", 0);

        System.out.println(hashMap);
        System.out.println("nickname:" + hashMap.get("nickname"));
        System.out.println(hashMap.containsKey("vip"));
        System.out.println(hashMap.keySet());
        System.out.println(hashMap.isEmpty());

        hashMap.remove("vip");
        System.out.println(hashMap.containsKey("cn"));

        //采用Iterator遍历HashMap
        Iterator it = hashMap.keySet().iterator();
        while (it.hasNext()) {
            String key = (String) it.next();
            System.out.println("key:" + key);
            System.out.println("value:" + hashMap.get(key));
        }

        //遍历HashMap的另一个方法
        Set<Map.Entry<String, Object>> sets = hashMap.entrySet();
        for (Map.Entry<String, Object> entry : sets) {
            System.out.print(entry.getKey() + ", ");
            System.out.println(entry.getValue());
        }
    }


}


```