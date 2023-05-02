Download Link: https://assignmentchef.com/product/solved-cpe348-project1-crc-calculation-and-ip-checksum-calculation
<br>
<strong>Part 1  CRC calculation.  </strong>The method for determining the CRC value to append to the message sent was discussed in class.  For the method shown in class, extra 0’s were added on to the original message before the calculation took place.

For this part of the project, show that by adding 1’s instead of 0’s results in the same CRC value added to the end of the message.  Remember that all math is binary XOR and no bits carry. To show that the same CRC value is added, you will have to perform 2 calculations to obtain the two messages sent – one calculation is for adding 0’s the other for adding 1’s.  Give the <strong>transmitted message</strong> from both calculations.

The message and generator to use for this project are shown below:

M(X) = 1001110011000011

C(X) = 11011

Reference textbook chapter 2, problem 20 for a more in-depth discussion of how CRC’s are actually calculated. Part a is a direct application of the above concept

Hint: The first part of the division is the same for the two calculations – only difference comes when you start bringing down the added in 0’s or 1’s.

<strong>Turn in all of your work on paper showing all of the calculations.  Using Excel will make it easier to keep the columns lined up</strong>.

<strong>Part2 IP checksum calculation.  </strong>For this part, perform the IP Checksum (use 16-bit checksum) on the following two IP headers.  If you do this by hand, be very neat and show all of your work.  If you use a program, print out the program and submit with your assignment<strong>.  </strong>

The IP header consists of 20 bytes of data.  This information is shown as hexadecimal numbers.  For example, look at the third grouping in the IP header in part a.  This grouping is <strong>bfc5</strong> and it is underlined. That grouping is hex digits b, f, c and 5 and in binary those hexadecimal digits are 1011, 1111, 1100 and 0101.  To calculate the checksum the <strong>Hex values or their binary equivalents can be added. </strong>

The header checksum value is shown in the shaded part of the header.  This checksum is calculated from the other parts of the header when a value of 0000 is used for the checksum field during the calculation.

For the first two IP headers shown, one of the checksums is correct.  The other checksum is incorrect. Compare your checksum result to the value for the checksum provided in the IP header.  Determine if the header was successfully received (do the checksums match?)

Use the example on the link shown to help with this problem: <a href="https://www.thegeekstuff.com/2012/05/ip-header-checksum/">https://www.thegeekstuff.com/2012/05/ip</a><a href="https://www.thegeekstuff.com/2012/05/ip-header-checksum/">header</a><a href="https://www.thegeekstuff.com/2012/05/ip-header-checksum/">–</a><a href="https://www.thegeekstuff.com/2012/05/ip-header-checksum/">checksum/</a>




<ol>

 <li>IP header to perform IP checksum on:</li>

</ol>

<strong>6500 0034 <u>bfc5</u> 4020 80a1 ab62 2db2 a50f 6f3a a80a</strong>

<ol>

 <li>IP header to perform IP checksum on:</li>

</ol>

<strong>6540 004e 39d6 6030 f0f6 DCC7 a9a8 aadd f265 ebbf </strong>

<ol>

 <li><strong>For 548 students only, </strong>determine the IP checksum for the following header</li>

</ol>

<h1>6560   f082 fa61 fa01 ffb6 ???? f9df ffdc f6c8 d2ff</h1>




Note: there is a c program in the textbook (pg 95) which can be programmed to calculate the checksum – provided you can have it successfully read in the hex digits (will require some extra work


