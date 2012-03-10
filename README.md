SunCalc-Java
=============

*This is a Java port of [https://github.com/mourner/suncalc](https://github.com/mourner/suncalc)*

Author: Nolan Caudill
License: BSD

Example usage:

```java
SunCalc.getPosition(new Date(1330560000), 33.0, -120.1);
System.out.println("azimuth: " + Double.toString(res.get("azimuth")));
System.out.println("altitude: " + Double.toString(res.get("altitude")));

Map<String, Date> res2 = SunCalc.getTimes(new Date(1330560000), 33.0, -120.1);
String[] res2_keys = res2.keySet().toArray(new String[0]);

for(int i = 0; i < res2_keys.length; i++) {
    System.out.println(res2_keys[i] + " " + res2.get(res2_keys[i]));
}
```

Note: This is the first Java I've written in about a dozen years so it might not be idiomatic, or I may have missed a short cut or two.
