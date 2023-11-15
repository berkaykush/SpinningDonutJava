# SpinningDonutJava

![Programming-Language-Java](https://img.shields.io/badge/Programming_Language-Java-brown.svg)
![Java-Version-17](https://img.shields.io/badge/Java_Version-17-blue.svg)
![Status-Complete](https://img.shields.io/badge/Status-Complete-green.svg)

Donut-shaped Java code that generates a 3D spinning donut.\
[Original C code(donut.c) and its explanation](https://www.a1k0n.net/2011/07/20/donut-math.html) written by Andy Sloane.

## Run with

While inside the `src` folder, run `javac main/java/com/donut/spinning/DonutShapedCode.java` and then \
`java main.java.com.donut.spinning.DonutShapedCode` in your terminal.

🍩 `DonutShapedCode.java`

```java
                package main.java.com.donut
           .spinning; import java.util.Arrays;
         public class DonutShapedCode{public static
       void main(String[] args){int k;double A=0,B=0,
     i,j; double[]z=new double[1760];char[]b=new char[
    1760]; System.out.print("\u001b[2J");for(;;){Arrays.
   fill(b,0,1760,' '); Arrays.fill(z,0,1760,0);for(j=0;j<
   6.28;j+=0.002) {for(i=0;i<6.28;i+=0.05){double c=Math.
   sin(i),d=Math.cos(j),e=        Math.sin(A),f=Math.sin(
  j),g=Math.cos(A),h=d+2,          D=1/( c*h*e+f*g+5 ),l=
  Math.cos(i),m=Math.cos(          B),n=Math.sin(B),t=c*h*
   g-f*e;int x=(int)(40+30        *D*(l*h*m-t*n)),y=(int)
   (12+15*D*(l*h*n+t*m)),o=x+80*y,N=(int)(8*((f*e-c*d*g)*
   m-c*d*e-f*g-l*d*n));if(22>y&&y>0&&80>x&&D>z[o]){z[o]=D
    ;b[o]=".,-~:;=!*#&@".charAt(Math.max(N,0));}}}System
      .out.print("\u001b[H");for(k=0;k<1761;k++){System
       .out.print((k%80)>0?b[k]:10);}A+=0.04;B+=0.02;
         }}}/*****####*******!!=;:~~::==!!!********
            **!!!==::-.,~~;;;========;;;~-...,-
                -.........................*/
```

https://github.com/berkaykush/SpinningDonutJava/assets/70837975/11f39e3b-39c2-4a41-903e-ff5a83c5350f
