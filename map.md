## map 的概念
格式 
interface Map<K,V> K 是键， v是值
不能有重复的键，一个键映射到一个值上
创建map 需要用 HashMap
eg
Map<String,String> Hs = new HashMap<String,String>();

Hs.put("key","value"); 用put的方法可以加入内容
如果加入重复的键，第二次出现的会替代掉新的内容

## 基本功能
put, remove(key) , clear(), containsKey, containsValue, isEmpty(), size();

## 获取功能
get(key) = value 根据键返回值
keySet() 返回键的集合
values() 返回值得集合

## 遍历方法
1. 

      Map<String,String> mp = new HashMap<String,String>();
      Set<String> keySet = map.keySet();
      for (String key:keySet){
        String value = map.get(key);
        sout(key + "," + value);
      }
    }

2. 
用entrySet 来获得键值对的集合

    Set<Map.Entry<String, String>> entrySet = map.entrySet();
    for(Map.Entry<String, String> me : entrySet){
      String key = me.getKey();
      String value = me.getValue();
      Sout(key + "," + value;
    }
    

    
