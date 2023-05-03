Download Link: https://assignmentchef.com/product/solved-cs-52-assignment-10-2
<br>
<strong>Questions:</strong> Using the page below, answer these questions.

<h4>1.  Look at the following examples and write your answer in the column next to the example.</h4>




<table border="1" width="100%">

 <tbody>

  <tr>

   <td width="50%">char * name1 = new char[ 6 ];strcpy( name1, “Henry” );char * name2 = name1;name1[0] = ‘D’;</td>

   <td width="50%">char s1[] = “The rain in Spain falls mainly on the plain.”char s2[] = “Hello, World!”;s1[12]=s2[0];s2[7] = s1[12];</td>

  </tr>

  <tr>

   <td width="50%">after executing the values of name1 and name2 will be:name1 = ____________________name2 = ____________________</td>

   <td width="50%">after executing the values of s1 and s2 will be:s1 = ____________________s2 = ____________________</td>

  </tr>

 </tbody>

</table>

<strong>2.  </strong>A program includes the following variable declarations:int  i1, i2;int *p1,*p2;List the output produced by the following code sample.  In addition, using the examples from class, draw a memory diagram showing the 4 variables i1, i2, p1 and p2.  Make sure the pointers have a link to the addresses they point to!  Draw these diagrams to show the memory state as things change

<table width="839">

 <tbody>

  <tr>

   <td width="249"><strong>Code Sample</strong></td>

   <td width="289"><strong>Output Generated By The Program</strong></td>

   <td width="287"><strong>Memory Diagram As Things Change</strong></td>

  </tr>

  <tr>

   <td width="249">i1 = 8;i2 = 9;p1 = &amp;i1;p2 = &amp;i2; cout &lt;&lt; “*p1=” &lt;&lt; *p1 &lt;&lt; endl;cout &lt;&lt; “*p2=” &lt;&lt; *p2 &lt;&lt; endl;*p1 = 10;*p2 = *p1;cout &lt;&lt; “i1=” &lt;&lt; i1 &lt;&lt; endl;cout &lt;&lt; “i2=” &lt;&lt; i2 &lt;&lt; endl;p2 = p1;*p2 = 11;cout &lt;&lt; “*p1=” &lt;&lt; *p1 &lt;&lt; endl;cout &lt;&lt; “*p2=” &lt;&lt; *p2 &lt;&lt; endl;</td>

   <td width="289"></td>

   <td width="287"><img decoding="async" width="200" height="150" data-recalc-dims="1" data-src="https://i0.wp.com/www.howardstahl.com/cs52/diagram1.jpg?resize=200%2C150" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

    <noscript>

     <img decoding="async" src="https://i0.wp.com/www.howardstahl.com/cs52/diagram1.jpg?resize=200%2C150" width="200" height="150" data-recalc-dims="1">

    </noscript>        </td>

  </tr>

 </tbody>

</table>

<strong>3. </strong>A program includes the following variable declarations:double  d1, d2;double *pd1,*pd2;List the output produced by the following code sample.  In addition, using the examples from class, draw a memory diagram showing the 4 variables d1, d2, pd1 and pd2.  Make sure the pointers have a link to the addresses they point to!  Draw these diagrams to show the memory state as things change.

<table width="85%">

 <tbody>

  <tr>

   <td><strong>Code Sample</strong></td>

   <td><strong>Output Generated By The Program</strong></td>

   <td><strong>Memory Diagram As Things Change</strong></td>

  </tr>

  <tr>

   <td>d1 = 12.4;d2 = 8.9;pd1 = &amp;d1;pd2 = &amp;d2; *pd1 = *pd2;*pd2 = 41.6;d2 = 13.4;cout &lt;&lt; “d1=” &lt;&lt; d1 &lt;&lt; endl;cout &lt;&lt; “d2=” &lt;&lt; d2 &lt;&lt; endl;</td>

   <td></td>

   <td><img decoding="async" width="200" height="150" data-recalc-dims="1" data-src="https://i0.wp.com/www.howardstahl.com/cs52/diagram2.jpg?resize=200%2C150" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

    <noscript>

     <img decoding="async" src="https://i0.wp.com/www.howardstahl.com/cs52/diagram2.jpg?resize=200%2C150" width="200" height="150" data-recalc-dims="1">

    </noscript>    </td>

  </tr>

 </tbody>

</table>

<strong>4.</strong>  For each variable listed on the left, determine whether that variable must deleted to prevent memory problems.  If so, state the appropriate delete statement necessary to destroy the dynamic variable and return the memory it uses to the heap so that other variables may use this memory.  Please assume that the following constant declarations have been made:const int  SIZE = 100;

<table width="95%">

 <tbody>

  <tr>

   <td>

    <table width="874">

     <tbody>

      <tr>

       <td width="366"><strong>Dynamic Variable Declaration</strong></td>

       <td width="204"><strong>Must Be Delete( ) ‘ed?</strong></td>

       <td width="290"><strong>Appropriate delete( ) Statement</strong></td>

      </tr>

      <tr>

       <td width="366">char * c = new char(‘b’);</td>

       <td width="204">yes no</td>

       <td width="290"></td>

      </tr>

      <tr>

       <td width="366">int i( 7 );</td>

       <td width="204">yes no</td>

       <td width="290"></td>

      </tr>

      <tr>

       <td width="366">double * d = new double( 12.1 );</td>

       <td width="204">yes no</td>

       <td width="290"></td>

      </tr>

      <tr>

       <td width="366">Student * s = new Student(“you”);</td>

       <td width="204">yes no</td>

       <td width="290"></td>

      </tr>

      <tr>

       <td width="366">double doubleArray [ SIZE ];</td>

       <td width="204">yes no</td>

       <td width="290"></td>

      </tr>

      <tr>

       <td width="366">int *intArray = new int[ 5 ];</td>

       <td width="204">yes no</td>

       <td width="290"></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Your submission should follow this organization:

  <ul>

   <li>part_a

    <ul>

     <li>responses.txt</li>

     <li>q2_step_diagram.pdf</li>

     <li>q3_step_diagram.pdf</li>

    </ul></li>

  </ul></li>

</ul>