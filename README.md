# ex
example codes

package ex;
import java.util.LinkedList;import java.util.StringTokenizer;
public class GetMinMaxString {  public String getMinMaxString(String str) {        StringTokenizer token = new StringTokenizer(str);        LinkedList<String> a = new LinkedList<String>();        String min="1000000";        String max="0";
        while(token.hasMoreTokens()) {         a.add(token.nextToken());        }          for(int i =0; i<a.size(); i++) {         if(Integer.parseInt(min) > Integer.parseInt(a.get(i)))          min = a.get(i);                   if(Integer.parseInt(max) < Integer.parseInt(a.get(i)))          max = a.get(i);        }                 return max +" "+ min;     }}
