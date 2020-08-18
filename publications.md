---
layout: default
title: Publications
section_id: portfolio
---

<div class="full parallax" style="background-image: url(images/banner/banner.jpg); color: #fff;">
  <div class="row">
    <div class="large-12 columns">
      {% include section-header.html title="Publications" tagline="Publications from the IRL Group" color="#000000" class="big" %}
    </div>
  </div>
  <div class="four spacing"></div>
</div>

<div class="row">
    <h2>COPYRIGHT NOTICE</h2>

    <p>
      The documents here are provided as a means to ensure timely dissemination of technical work on a noncommercial basis. Copyright and all rights therein are maintained by the authors or by other copyright holders. It is understood that anyone copying the papers from this page will adhere to the terms and constraints invoked by the copyright.
    </p>
</div>

<div class="row">

{% assign current_year = site.time | date: "%Y" %}
{% assign months = "January,February,March,April,May,June,July,August,September,October,November,December" | split: "," %}
{% for year in (2018..current_year) reversed %}
  <h3>{{ year }}</h3>
  <ul>
  {% for month in months reversed %}
    {% for pub in site.data.publications %}
      {% assign pub_month_downcase = pub.month | downcase %}
      {% assign month_downcase = month | downcase %}
      {% if pub.year == year and pub_month_downcase == month_downcase %}
        {% if pub.type == "conference" or pub.type == "journal" or pub.type == "preprint" %}
          <li>
          {% if pub.type == "conference" %}
            {{ pub.authors }}<br />
            <strong>"{{ pub.title }}"</strong><br />
            <em>{{ pub.conference }}</em>, {{ month }} {{ year }}.<br />
          {% elsif pub.type == "journal" %}
            {{ pub.authors }}<br />
            <strong>"{{ pub.title }}"</strong><br />
            <em>{{ pub.journal }}</em>, vol. {{ pub.volume }}, {% if pub.issue %}no. {{ pub.issue }}, {% endif %}pp. {{ pub.pages }}, {{ month }} {{ year }}.<br />
          {% elsif pub.type == "preprint" %}
            {{ pub.authors }}<br />
            <strong>"{{ pub.title }}"</strong><br />
            <em>{{ pub.archive }}</em> preprint {{ pub.number }}, {{ month }} {{ year }}.<br />
          {% endif %}
          {% if pub.note %}
          <em>{{ pub.note }}</em><br />
          {% endif %}
          {% if pub.pdf %}
            <a href="data/files/papers/{{ pub.pdf }}" target="_blank"><img src="images/extensions/pdf.png" alt="PDF" /></a>
          {% elsif pub.pdfext %}
            <a href="{{ pub.pdfext }}" target="_blank"><img src="images/extensions/pdf.png" alt="PDF" /></a>
          {% endif %}
          </li>
        {% endif %}
      {% endif %}
    {% endfor %}
  {% endfor %}
  </ul>
{% endfor %}

<h3>2017</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=278" title="Kevin Chan, Bongjun Ko, Spyridon Mastorakis, Alexander Afanasyev, and Lixia Zhang, &lt;strong&gt;&amp;quot;Fuzzy Interest Forwarding&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of Asian Internet Engineering Conference (AINTEC)&lt;/em&gt;, November  2017. "><img src="/images/extensions/bib.png" /></a>

     Kevin Chan, Bongjun Ko, Spyridon Mastorakis, Alexander Afanasyev, and Lixia Zhang, <br/><strong>&quot;Fuzzy Interest Forwarding</strong>,&quot; <br/>in <em>Proceedings of Asian Internet Engineering Conference (AINTEC)</em>, November  2017.

        <a target="_blank" href="/data/files/papers/chan2017fuzzy.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=271" title="Yu Yingdi, Alexander Afanasyev, Jan Seedorf, Zhiyi Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;NDN DeLorean: An authentication system for data archives in named data networking&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 4th ACM Conference on Information-Centric Networking&lt;/em&gt;, September  2017, pp. 11&amp;ndash;21. "><img src="/images/extensions/bib.png" /></a>

     Yu Yingdi, Alexander Afanasyev, Jan Seedorf, Zhiyi Zhang, and Lixia Zhang, <br/><strong>&quot;NDN DeLorean: An authentication system for data archives in named data networking</strong>,&quot; <br/>in <em>Proceedings of the 4th ACM Conference on Information-Centric Networking</em>, September  2017, pp. 11&ndash;21.

        <a target="_blank" href="/data/files/papers/icn-delorean-17.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=256" title="Christopher Gibson, Pablo Bermell-Garcia, Kevin Chan, Bongjun Ko, Alex Afanasyev, and Lixia Zhang, &lt;strong&gt;&amp;quot;Opportunities and Challenges for Named Data Networking to Increase the Agility of Military Coalitions&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of Workshop on Distributed Analytics InfraStructure and Algorithms for Multi-Organization Federations (DAIS)&lt;/em&gt;, August  2017. "><img src="/images/extensions/bib.png" /></a>

     Christopher Gibson, Pablo Bermell-Garcia, Kevin Chan, Bongjun Ko, Alex Afanasyev, and Lixia Zhang, <br/><strong>&quot;Opportunities and Challenges for Named Data Networking to Increase the Agility of Military Coalitions</strong>,&quot; <br/>in <em>Proceedings of Workshop on Distributed Analytics InfraStructure and Algorithms for Multi-Organization Federations (DAIS)</em>, August  2017.


    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=257" title="Spyridon Mastorakis, Alexander Afanasyev, Yingdi Yu, and Lixia Zhang, &lt;strong&gt;&amp;quot;NTorrent: Peer-to-Peer File Sharing in Named Data Networking&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 26th International Conference on Computer Communications and Networks (ICCCN)&lt;/em&gt;, July  2017. "><img src="/images/extensions/bib.png" /></a>

     Spyridon Mastorakis, Alexander Afanasyev, Yingdi Yu, and Lixia Zhang, <br/><strong>&quot;NTorrent: Peer-to-Peer File Sharing in Named Data Networking</strong>,&quot; <br/>in <em>Proceedings of the 26th International Conference on Computer Communications and Networks (ICCCN)</em>, July  2017.


    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=258" title="Alexander Afanasyev, Xiaoke Jiang, Yingdi Yu, Jiewen Tan, Yumin Xia, Allison Mankin, and Lixia Zhang, &lt;strong&gt;&amp;quot;NDNS: A DNS-Like Name Service for NDN&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 26th International Conference on Computer Communications and Networks (ICCCN)&lt;/em&gt;, July  2017. "><img src="/images/extensions/bib.png" /></a>

     Alexander Afanasyev, Xiaoke Jiang, Yingdi Yu, Jiewen Tan, Yumin Xia, Allison Mankin, and Lixia Zhang, <br/><strong>&quot;NDNS: A DNS-Like Name Service for NDN</strong>,&quot; <br/>in <em>Proceedings of the 26th International Conference on Computer Communications and Networks (ICCCN)</em>, July  2017.


    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=286" title="Spyridon Mastorakis, Alexander Afanasyev, and Lixia Zhang, &lt;strong&gt;&amp;quot;On the Evolution of ndnSIM: an Open-Source Simulator for NDN Experimentation&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM Computer Communication Review&lt;/em&gt;, July  2017. "><img src="/images/extensions/bib.png" /></a>

     Spyridon Mastorakis, Alexander Afanasyev, and Lixia Zhang, <br/><strong>&quot;On the Evolution of ndnSIM: an Open-Source Simulator for NDN Experimentation</strong>,&quot; <br/><em>ACM Computer Communication Review</em>, July  2017.

        <a target="_blank" href="/data/files/papers/ccr17-ndnsim.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=287" title="Alexander Afanasyev, Xiaoke Jiang, Yingdi Yu, Jiewen Tan, Yumin Xia, Allison Mankin, and Lixia Zhang, &lt;strong&gt;&amp;quot;NDNS: DNS-like Name Service for NDN&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 26th International Conference on Computer Communications and Networks (ICCCN)&lt;/em&gt;, July  2017. "><img src="/images/extensions/bib.png" /></a>

     Alexander Afanasyev, Xiaoke Jiang, Yingdi Yu, Jiewen Tan, Yumin Xia, Allison Mankin, and Lixia Zhang, <br/><strong>&quot;NDNS: DNS-like Name Service for NDN</strong>,&quot; <br/>in <em>Proceedings of the 26th International Conference on Computer Communications and Networks (ICCCN)</em>, July  2017.

        <a target="_blank" href="/data/files/papers/2017-icccn-ndns.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=288" title="Spyridon Mastorakis, Alexander Afanasyev, Yingdi Yu, and Lixia Zhang, &lt;strong&gt;&amp;quot;NTorrent: Peer-to-peer File Sharing in Named Data Networking&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 26th International Conference on Computer Communications and Networks (ICCCN)&lt;/em&gt;, July  2017. "><img src="/images/extensions/bib.png" /></a>

     Spyridon Mastorakis, Alexander Afanasyev, Yingdi Yu, and Lixia Zhang, <br/><strong>&quot;NTorrent: Peer-to-peer File Sharing in Named Data Networking</strong>,&quot; <br/>in <em>Proceedings of the 26th International Conference on Computer Communications and Networks (ICCCN)</em>, July  2017.

        <a target="_blank" href="/data/files/papers/2017-icccn-ntorrent.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=259" title="Wentao Shang, Zhehao Wang, Alexander Afanasyev, Jeff Burke, and Lixia Zhang, &lt;strong&gt;&amp;quot;Breaking out of the Cloud: Local Trust Management and Rendezvous in Named Data Networking of Things&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 2nd ACM/IEEE International Conference on Internet-of-Things Design and Implementation (IoTDI)&lt;/em&gt;, Pittsburgh, PA, USA, April  2017. "><img src="/images/extensions/bib.png" /></a>

     Wentao Shang, Zhehao Wang, Alexander Afanasyev, Jeff Burke, and Lixia Zhang, <br/><strong>&quot;Breaking out of the Cloud: Local Trust Management and Rendezvous in Named Data Networking of Things</strong>,&quot; <br/>in <em>Proceedings of the 2nd ACM/IEEE International Conference on Internet-of-Things Design and Implementation (IoTDI)</em>, Pittsburgh, PA, USA, April  2017.


    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=289" title="Wentao Shang, Zhehao Wang, Alexander Afanasyev, Jeff Burke, and Lixia Zhang, &lt;strong&gt;&amp;quot;Breaking out of the Cloud: Local Trust Management and Rendezvous in Named Data Networking of Things&lt;/strong&gt;,&amp;quot; in &lt;em&gt;ACM/IEEE International Conference on Internet-of-Things Design and Implementation (IoTDI)&lt;/em&gt;, April  2017. "><img src="/images/extensions/bib.png" /></a>

     Wentao Shang, Zhehao Wang, Alexander Afanasyev, Jeff Burke, and Lixia Zhang, <br/><strong>&quot;Breaking out of the Cloud: Local Trust Management and Rendezvous in Named Data Networking of Things</strong>,&quot; <br/>in <em>ACM/IEEE International Conference on Internet-of-Things Design and Implementation (IoTDI)</em>, April  2017.

        <a target="_blank" href="/data/files/papers/ndn-breaking-out-of-cloud-IOTDI-2017.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2016</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=252" title="Wentao Shang, Alexander Afanasyev, and Lixia Zhang, &lt;strong&gt;&amp;quot;The Design and Implementation of the NDN Protocol Stack for RIOT-OS&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of GLOBECOM Workshop on Information Centric Networking Solutions for Real World Applications (ICNSRA)&lt;/em&gt;, December  2016. "><img src="/images/extensions/bib.png" /></a>

     Wentao Shang, Alexander Afanasyev, and Lixia Zhang, <br/><strong>&quot;The Design and Implementation of the NDN Protocol Stack for RIOT-OS</strong>,&quot; <br/>in <em>Proceedings of GLOBECOM Workshop on Information Centric Networking Solutions for Real World Applications (ICNSRA)</em>, December  2016.

        <a target="_blank" href="/data/files/papers/globecom-icnsra16-ndn-riot.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=253" title="Alexander Afanasyev, Alex J. Halderman, Scott Ruoti, Kent Seamons, Yingdi Yu, Daniel Zappala, and Lixia Zhang, &lt;strong&gt;&amp;quot;Content-Based Security for the Web&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of New Security Paradigms Workshop (NSPW)&lt;/em&gt;, September  2016. "><img src="/images/extensions/bib.png" /></a>

     Alexander Afanasyev, Alex J. Halderman, Scott Ruoti, Kent Seamons, Yingdi Yu, Daniel Zappala, and Lixia Zhang, <br/><strong>&quot;Content-Based Security for the Web</strong>,&quot; <br/>in <em>Proceedings of New Security Paradigms Workshop (NSPW)</em>, September  2016.

        <a target="_blank" href="/data/files/papers/nspw16-cbsec-web.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=231" title="Wentao Shang, Adeola Bannis, Teng Liang, Zhehao Wang, Yingdi Yu, Alexander Afanasyev, Jeff Thompson, Jeff Burke, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Named Data Networking of Things&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of 1st IEEE International Conference on Internet-of-Things Design and Implementation (IoTDI&#039;2016)&lt;/em&gt;, April  2016. (Invited paper)"><img src="/images/extensions/bib.png" /></a>

     Wentao Shang, Adeola Bannis, Teng Liang, Zhehao Wang, Yingdi Yu, Alexander Afanasyev, Jeff Thompson, Jeff Burke, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Named Data Networking of Things</strong>,&quot; <br/>in <em>Proceedings of 1st IEEE International Conference on Internet-of-Things Design and Implementation (IoTDI'2016)</em>, April  2016. (Invited paper)

        <a target="_blank" href="/data/files/papers/iotdi16-ndn-of-things.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=250" title="Yu Zhang, Alexander Afanasyev, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Survey of Mobility Support in Named Data Networking&lt;/strong&gt;,&amp;quot; &lt;em&gt;Proceedings of the third Workshop on Name-Oriented Mobility: Architecture, Algorithms and Applications (NOM’2016)&lt;/em&gt;, April  2016. "><img src="/images/extensions/bib.png" /></a>

     Yu Zhang, Alexander Afanasyev, and Lixia Zhang, <br/><strong>&quot;A Survey of Mobility Support in Named Data Networking</strong>,&quot; <br/><em>Proceedings of the third Workshop on Name-Oriented Mobility: Architecture, Algorithms and Applications (NOM’2016)</em>, April  2016.

        <a target="_blank" href="/data/files/papers/nom16-ndn-mobility-survey.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=230" title="Alexander Afanasyev, Yingdi Yu, Lixia Zhang, Jeff Burke, kc claffy, and Joshua Polterock, &lt;strong&gt;&amp;quot;The Second Named Data Networking Community Meeting (NDNcomm 2015)&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM Computer Communication Review&lt;/em&gt;, 2016. "><img src="/images/extensions/bib.png" /></a>

     Alexander Afanasyev, Yingdi Yu, Lixia Zhang, Jeff Burke, kc claffy, and Joshua Polterock, <br/><strong>&quot;The Second Named Data Networking Community Meeting (NDNcomm 2015)</strong>,&quot; <br/><em>ACM SIGCOMM Computer Communication Review</em>, 2016.

        <a target="_blank" href="/data/files/papers/ccr16-2nd-ndncomm.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2015</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=229" title="Alexander Afanasyev, Zhenkai Zhu, and Lixia Zhang, &lt;strong&gt;&amp;quot;The Story of ChronoShare, or How NDN Brought Distributed Secure File Sharing Back&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE MASS 2015 Workshop on Content-Centric Networks&lt;/em&gt;, October  2015. "><img src="/images/extensions/bib.png" /></a>

     Alexander Afanasyev, Zhenkai Zhu, and Lixia Zhang, <br/><strong>&quot;The Story of ChronoShare, or How NDN Brought Distributed Secure File Sharing Back</strong>,&quot; <br/>in <em>Proceedings of IEEE MASS 2015 Workshop on Content-Centric Networks</em>, October  2015.

        <a target="_blank" href="/data/files/papers/mass15-chronoshare.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=228" title="Yingdi Yu, Alexander Afanasyev, David Clark, kc claffy, Van Jacobson, and Lixia Zhang, &lt;strong&gt;&amp;quot;Schematizing and Automating Trust in Named Data Networking&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of 2nd ACM Conference on Information-Centric Networking&lt;/em&gt;, September  2015. "><img src="/images/extensions/bib.png" /></a>

     Yingdi Yu, Alexander Afanasyev, David Clark, kc claffy, Van Jacobson, and Lixia Zhang, <br/><strong>&quot;Schematizing and Automating Trust in Named Data Networking</strong>,&quot; <br/>in <em>Proceedings of 2nd ACM Conference on Information-Centric Networking</em>, September  2015.

        <a target="_blank" href="/data/files/papers/icn15-trust-schema.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=232" title="Ilya Moiseenko, Lijing Wang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Consumer/producer communication with application level framing in Named Data Networking&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 2nd International Conference on Information-Centric Networking&lt;/em&gt;, September  2015, pp. 99&amp;ndash;108. "><img src="/images/extensions/bib.png" /></a>

     Ilya Moiseenko, Lijing Wang, and Lixia Zhang, <br/><strong>&quot;Consumer/producer communication with application level framing in Named Data Networking</strong>,&quot; <br/>in <em>Proceedings of the 2nd International Conference on Information-Centric Networking</em>, September  2015, pp. 99&ndash;108.

        <a target="_blank" href="/data/files/papers/icn15-consumer-producer.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=224" title="kc claffy, Josh Polterock, Alexander Afanasyev, Jeff Burke, and Lixia Zhang, &lt;strong&gt;&amp;quot;The First Named Data Networking Community Meeting (NDNcomm)&lt;/strong&gt;,&amp;quot; &lt;em&gt;In submission to ACM SIGCOMM Computer Communication Review (CCR)&lt;/em&gt;, April  2015. "><img src="/images/extensions/bib.png" /></a>

     kc claffy, Josh Polterock, Alexander Afanasyev, Jeff Burke, and Lixia Zhang, <br/><strong>&quot;The First Named Data Networking Community Meeting (NDNcomm)</strong>,&quot; <br/><em>In submission to ACM SIGCOMM Computer Communication Review (CCR)</em>, April  2015.

        <a target="_blank" href="/data/files/papers/ccr15-1st-ndncomm.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=225" title="Alexander Afanasyev, Cheng Yi, Lan Wang, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;SNAMP: Secure Namespace Mapping to Scale NDN Forwarding&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of 18th IEEE Global Internet Symposium (GI 2015)&lt;/em&gt;, April  2015. "><img src="/images/extensions/bib.png" /></a>

     Alexander Afanasyev, Cheng Yi, Lan Wang, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;SNAMP: Secure Namespace Mapping to Scale NDN Forwarding</strong>,&quot; <br/>in <em>Proceedings of 18th IEEE Global Internet Symposium (GI 2015)</em>, April  2015.

        <a target="_blank" href="/data/files/papers/gi15-snamp.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=226" title="Weiqi Shi and Alexander Afanasyev, &lt;strong&gt;&amp;quot;RepoSync: Combined Action-Based and Data-Based Synchronization Model in Named Data Network&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of 18th IEEE Global Internet Symposium (GI 2015)&lt;/em&gt;, April  2015. "><img src="/images/extensions/bib.png" /></a>

     Weiqi Shi and Alexander Afanasyev, <br/><strong>&quot;RepoSync: Combined Action-Based and Data-Based Synchronization Model in Named Data Network</strong>,&quot; <br/>in <em>Proceedings of 18th IEEE Global Internet Symposium (GI 2015)</em>, April  2015.

        <a target="_blank" href="/data/files/papers/gi15-reposync.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2014</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=223" title="&lt;a href=\&quot;http://conferences2.sigcomm.org/acm-icn/2014/program.php\&quot; target=\&quot;_blank\&quot;&gt;&lt;img src=&#039;/images/extensions/php.png&#039; style=&#039;margin:0 5px 0 0; &#039; /&gt;&lt;/a&gt; Cheng Yi, Jerald Abraham, Alexander Afanasyev, Lan Wang, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;On the Role of Routing in Named Data Networking&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of ACM Conference on Information-Centric Networking (ICN&#039;2014)&lt;/em&gt;, September  2014. "><img src="/images/extensions/bib.png" /></a>

     <a href="http://conferences2.sigcomm.org/acm-icn/2014/program.php" target="_blank"><img src='/images/extensions/php.png' style='margin:0 5px 0 0; ' /></a> Cheng Yi, Jerald Abraham, Alexander Afanasyev, Lan Wang, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;On the Role of Routing in Named Data Networking</strong>,&quot; <br/>in <em>Proceedings of ACM Conference on Information-Centric Networking (ICN'2014)</em>, September  2014.

        <a target="_blank" href="/data/files/papers/icn14-on-the-role-of-routing-ndn.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2013</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=220" title="&lt;a href=\&quot;http://icnp13.informatik.uni-goettingen.de/index.html\&quot; target=\&quot;_blank\&quot;&gt;&lt;img src=&#039;/images/extensions/html.png&#039; style=&#039;margin:0 5px 0 0; &#039; /&gt;&lt;/a&gt; Zhenkai Zhu and Alexander Afanasyev, &lt;strong&gt;&amp;quot;Let&#039;s ChronoSync: Decentralized Dataset State Synchronization in Named Data Networking&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 21st IEEE International Conference on Network Protocols (ICNP 2013)&lt;/em&gt;, Goettingen, Germany, October  2013. "><img src="/images/extensions/bib.png" /></a>

     <a href="http://icnp13.informatik.uni-goettingen.de/index.html" target="_blank"><img src='/images/extensions/html.png' style='margin:0 5px 0 0; ' /></a> Zhenkai Zhu and Alexander Afanasyev, <br/><strong>&quot;Let's ChronoSync: Decentralized Dataset State Synchronization in Named Data Networking</strong>,&quot; <br/>in <em>Proceedings of the 21st IEEE International Conference on Network Protocols (ICNP 2013)</em>, Goettingen, Germany, October  2013.

        <a target="_blank" href="/data/files/papers/icnp2013-chronosync.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=217" title="Alexander Afanasyev, Priya Mahadevan, Ilya Moiseenko, Ersin Uzun, and Lixia Zhang, &lt;strong&gt;&amp;quot;Interest Flooding Attack and Countermeasures in Named Data Networking&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Accepted to IFIP Networking 2013&lt;/em&gt;, May  2013. "><img src="/images/extensions/bib.png" /></a>

     Alexander Afanasyev, Priya Mahadevan, Ilya Moiseenko, Ersin Uzun, and Lixia Zhang, <br/><strong>&quot;Interest Flooding Attack and Countermeasures in Named Data Networking</strong>,&quot; <br/>in <em>Accepted to IFIP Networking 2013</em>, May  2013.

        <a target="_blank" href="/data/files/papers/ifip-networking13-interest-flooding-ndn.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=218" title="Wentao Shang, Jeff Thompson, Meki Cherkaoui, Jeff Burke, and Lixia Zhang, &lt;strong&gt;&amp;quot;NDN.JS: A JavaScript Client Library for Named Data Networking&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE INFOCOMM 2013 NOMEN Workshop&lt;/em&gt;, April  2013. "><img src="/images/extensions/bib.png" /></a>

     Wentao Shang, Jeff Thompson, Meki Cherkaoui, Jeff Burke, and Lixia Zhang, <br/><strong>&quot;NDN.JS: A JavaScript Client Library for Named Data Networking</strong>,&quot; <br/>in <em>Proceedings of IEEE INFOCOMM 2013 NOMEN Workshop</em>, April  2013.

        <a target="_blank" href="/data/files/papers/nomen13-ndnjs.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=219" title="&lt;a href=\&quot;http://infocom.di.unimi.it/index.php/tmaprogram.html\&quot; target=\&quot;_blank\&quot;&gt;&lt;img src=&#039;/images/extensions/html.png&#039; style=&#039;margin:0 5px 0 0; &#039; /&gt;&lt;/a&gt; Yingdi Yu, Duane Wessels, Matt Larson, and Lixia Zhang, &lt;strong&gt;&amp;quot;Check-R: A New Method of Measuring DNSSEC Validating Resolvers&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of INFOCOM 2013 Workshop on Traffic Measurement Analysis&lt;/em&gt;, April  2013. "><img src="/images/extensions/bib.png" /></a>

     <a href="http://infocom.di.unimi.it/index.php/tmaprogram.html" target="_blank"><img src='/images/extensions/html.png' style='margin:0 5px 0 0; ' /></a> Yingdi Yu, Duane Wessels, Matt Larson, and Lixia Zhang, <br/><strong>&quot;Check-R: A New Method of Measuring DNSSEC Validating Resolvers</strong>,&quot; <br/>in <em>Proceedings of INFOCOM 2013 Workshop on Traffic Measurement Analysis</em>, April  2013.

        <a target="_blank" href="/data/files/papers/tma13-check-r-dnssec.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=216" title="&lt;a href=\&quot;http://dx.doi.org/10.1016/j.comcom.2013.01.005\&quot; target=\&quot;_blank\&quot;&gt;&lt;img src=&#039;/images/extensions/html.png&#039; style=&#039;margin:0 5px 0 0; &#039; /&gt;&lt;/a&gt; Cheng Yi, Alexander Afanasyev, Ilya Moiseenko, Lan Wang, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Case for Stateful Forwarding Plane&lt;/strong&gt;,&amp;quot; &lt;em&gt;Computer Communications&lt;/em&gt;, vol. 36, no. 7, pp. 779&amp;ndash;791, 2013. ISSN 0140-3664"><img src="/images/extensions/bib.png" /></a>

     <a href="http://dx.doi.org/10.1016/j.comcom.2013.01.005" target="_blank"><img src='/images/extensions/html.png' style='margin:0 5px 0 0; ' /></a> Cheng Yi, Alexander Afanasyev, Ilya Moiseenko, Lan Wang, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;A Case for Stateful Forwarding Plane</strong>,&quot; <br/><em>Computer Communications</em>, vol. 36, no. 7, pp. 779&ndash;791, 2013. ISSN 0140-3664

        <a target="_blank" href="/data/files/papers/comcom-stateful-forwarding.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2012</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=210" title="Cheng Yi, Alexander Afanasyev, Lan Wang, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Adaptive Forwarding in Named Data Networking&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM Computer Communication Reviews&lt;/em&gt;, vol. 42, no. 3, pp. 62&amp;ndash;67, July  2012. "><img src="/images/extensions/bib.png" /></a>

     Cheng Yi, Alexander Afanasyev, Lan Wang, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Adaptive Forwarding in Named Data Networking</strong>,&quot; <br/><em>ACM Computer Communication Reviews</em>, vol. 42, no. 3, pp. 62&ndash;67, July  2012.

        <a target="_blank" href="/data/files/papers/ccr-ndn-adaptive-forwarding.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=202" title="P-C. Cheng, J-H. Park, K. Patel, S. Amante, and L. Zhang, &lt;strong&gt;&amp;quot;Explaining BGP Slow Table Transfers&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the International Conference on Distributed Computing Systems (ICDCS)&lt;/em&gt;, June  2012. "><img src="/images/extensions/bib.png" /></a>

     P-C. Cheng, J-H. Park, K. Patel, S. Amante, and L. Zhang, <br/><strong>&quot;Explaining BGP Slow Table Transfers</strong>,&quot; <br/>in <em>Proceedings of the International Conference on Distributed Computing Systems (ICDCS)</em>, June  2012.

        <a target="_blank" href="/data/files/papers/bgplimit.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=207" title="Lucas Wang, Alexander Afanasyev, Romain Kuntz, Rama Vuyyuru, Ryuji Wakikawa, and Lixia Zhang, &lt;strong&gt;&amp;quot;Rapid Traffic Information Dissemination Using Named Data&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 1st ACM workshop on Emerging Name-Oriented Mobile Networking Design-Architecture, Algorithms, and Applications (NoM&#039;12)&lt;/em&gt;, Hilton Head Island, South Carolina, June  2012, pp. 7&amp;ndash;12. "><img src="/images/extensions/bib.png" /></a>

     Lucas Wang, Alexander Afanasyev, Romain Kuntz, Rama Vuyyuru, Ryuji Wakikawa, and Lixia Zhang, <br/><strong>&quot;Rapid Traffic Information Dissemination Using Named Data</strong>,&quot; <br/>in <em>Proceedings of the 1st ACM workshop on Emerging Name-Oriented Mobile Networking Design-Architecture, Algorithms, and Applications (NoM'12)</em>, Hilton Head Island, South Carolina, June  2012, pp. 7&ndash;12.

        <a target="_blank" href="/data/files/papers/nom12-rapid-traffic.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=203" title="Yingdi Yu, Duane Wessels, Matt Larson, and Lixia Zhang, &lt;strong&gt;&amp;quot;Authority Server Selection of DNS Caching Resolvers&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM Computer Communication Reviews&lt;/em&gt;, April  2012. "><img src="/images/extensions/bib.png" /></a>

     Yingdi Yu, Duane Wessels, Matt Larson, and Lixia Zhang, <br/><strong>&quot;Authority Server Selection of DNS Caching Resolvers</strong>,&quot; <br/><em>ACM SIGCOMM Computer Communication Reviews</em>, April  2012.

        <a target="_blank" href="/data/files/papers/res_ns_selection.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=200" title="J-H. Park, P-C. Cheng, S. Amante, D. Kim, D. McPherson, and L. Zhang, &lt;strong&gt;&amp;quot;A Comparative Study of Architectural Impact on BGP Next-hop Diversity&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of 15th IEEE Global Internet Symposium (INFOCOM workshop)&lt;/em&gt;, March  2012. "><img src="/images/extensions/bib.png" /></a>

     J-H. Park, P-C. Cheng, S. Amante, D. Kim, D. McPherson, and L. Zhang, <br/><strong>&quot;A Comparative Study of Architectural Impact on BGP Next-hop Diversity</strong>,&quot; <br/>in <em>Proceedings of 15th IEEE Global Internet Symposium (INFOCOM workshop)</em>, March  2012.

        <a target="_blank" href="/data/files/papers/gi12-bgp-next-hop-diversity.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=204" title="Lucas Wang, Ryuji Wakikawa, Romain Kuntz, Rama Vuyyuru, and Lixia Zhang, &lt;strong&gt;&amp;quot;Data Naming in Vehicle-to-Vehicle Communications&lt;/strong&gt;,&amp;quot; in &lt;em&gt;In Proceedings of INFOCOM 2012 Workshop on Emerging Design Choices in Name-Oriented Networking&lt;/em&gt;, March  2012. "><img src="/images/extensions/bib.png" /></a>

     Lucas Wang, Ryuji Wakikawa, Romain Kuntz, Rama Vuyyuru, and Lixia Zhang, <br/><strong>&quot;Data Naming in Vehicle-to-Vehicle Communications</strong>,&quot; <br/>in <em>In Proceedings of INFOCOM 2012 Workshop on Emerging Design Choices in Name-Oriented Networking</em>, March  2012.

        <a target="_blank" href="/data/files/papers/data-naming-v2v.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=205" title="Basil Etefia and Lixia Zhang, &lt;strong&gt;&amp;quot;Named Data Networking for Military Communication Systems&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE Aerospace Conference&lt;/em&gt;, March  2012. "><img src="/images/extensions/bib.png" /></a>

     Basil Etefia and Lixia Zhang, <br/><strong>&quot;Named Data Networking for Military Communication Systems</strong>,&quot; <br/>in <em>Proceedings of IEEE Aerospace Conference</em>, March  2012.

        <a target="_blank" href="/data/files/papers/2012Milcom.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2011</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=197" title="Alexander Afanasyev, Jiangzhe Wang, Chunyi Peng, and Lixia Zhang, &lt;strong&gt;&amp;quot;Measuring redundancy level on the Web&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of Asian Internet Engineering Conference 2011 (AINTEC 2011)&lt;/em&gt;, November  2011. "><img src="/images/extensions/bib.png" /></a>

     Alexander Afanasyev, Jiangzhe Wang, Chunyi Peng, and Lixia Zhang, <br/><strong>&quot;Measuring redundancy level on the Web</strong>,&quot; <br/>in <em>Proceedings of Asian Internet Engineering Conference 2011 (AINTEC 2011)</em>, November  2011.

        <a target="_blank" href="http://lasr.cs.ucla.edu/afanasyev/data/files/Afanasyev/aintec-search.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=198" title="Zhenkai Zhu, Ryuji Wakikawa, Stuart Cheshire, and Lixia Zhang, &lt;strong&gt;&amp;quot;Home As You Go: An Engineering Approach to Mobility-Capable Extended Home Networks&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of Asian Internet Engineering Conference 2011 (AINTEC 2011)&lt;/em&gt;, November  2011. "><img src="/images/extensions/bib.png" /></a>

     Zhenkai Zhu, Ryuji Wakikawa, Stuart Cheshire, and Lixia Zhang, <br/><strong>&quot;Home As You Go: An Engineering Approach to Mobility-Capable Extended Home Networks</strong>,&quot; <br/>in <em>Proceedings of Asian Internet Engineering Conference 2011 (AINTEC 2011)</em>, November  2011.

        <a target="_blank" href="http://irl.cs.ucla.edu/~zhenkai/papers/btmm.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=206" title="Z. Zhu, J. Burke, L. Zhang, P. Gasti, Y. Lu, and V. Jacobson, &lt;strong&gt;&amp;quot;A new approach to securing audio conference tools&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 7th Asian Internet Engineering Conference&lt;/em&gt;, November  2011, pp. 120&amp;ndash;123. "><img src="/images/extensions/bib.png" /></a>

     Z. Zhu, J. Burke, L. Zhang, P. Gasti, Y. Lu, and V. Jacobson, <br/><strong>&quot;A new approach to securing audio conference tools</strong>,&quot; <br/>in <em>Proceedings of the 7th Asian Internet Engineering Conference</em>, November  2011, pp. 120&ndash;123.

        <a target="_blank" href="/data/files/papers/awfit-audiosec.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=169" title="Zhenkai Zhu, Sen Wang, Xu Yang, Van Jacobson, and Lixia Zhang, &lt;strong&gt;&amp;quot;ACT: Audio Conference Tool Over Named Data Networks&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of SIGCOMM 2011 Workshop on Information Centric Networking&lt;/em&gt;, August  2011. "><img src="/images/extensions/bib.png" /></a>

     Zhenkai Zhu, Sen Wang, Xu Yang, Van Jacobson, and Lixia Zhang, <br/><strong>&quot;ACT: Audio Conference Tool Over Named Data Networks</strong>,&quot; <br/>in <em>Proceedings of SIGCOMM 2011 Workshop on Information Centric Networking</em>, August  2011.

        <a target="_blank" href="/data/files/papers/icn10c-zhu.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=177" title="Dan Massey, Christos Papadopoulos, Lan Wang, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Teaching Network Architecture through case Studies&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of SIGCOMM 2011 Education workshop&lt;/em&gt;, August  2011. "><img src="/images/extensions/bib.png" /></a>

     Dan Massey, Christos Papadopoulos, Lan Wang, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Teaching Network Architecture through case Studies</strong>,&quot; <br/>in <em>Proceedings of SIGCOMM 2011 Education workshop</em>, August  2011.

        <a target="_blank" href="/data/files/papers/sigcomm11-teaching-network-arch.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=175" title="Zhenkai Zhu, Ryuji Wakikawa, and Lixia Zhang, &lt;strong&gt;&amp;quot;Supporting Mobility for Internet Cars&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Communication Magazine&lt;/em&gt;, May  2011. "><img src="/images/extensions/bib.png" /></a>

     Zhenkai Zhu, Ryuji Wakikawa, and Lixia Zhang, <br/><strong>&quot;Supporting Mobility for Internet Cars</strong>,&quot; <br/><em>IEEE Communication Magazine</em>, May  2011.

        <a target="_blank" href="http://irl.cs.ucla.edu/~zhenkai/InternetCarsDraft.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=176" title="Eric Osterweil, Danny McPherson, and Lixia Zhang, &lt;strong&gt;&amp;quot;Operational Implications of the DNS Control Plane&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Reliability Society Newsletter&lt;/em&gt;, May  2011. "><img src="/images/extensions/bib.png" /></a>

     Eric Osterweil, Danny McPherson, and Lixia Zhang, <br/><strong>&quot;Operational Implications of the DNS Control Plane</strong>,&quot; <br/><em>IEEE Reliability Society Newsletter</em>, May  2011.

        <a target="_blank" href="http://www.ieeereliability.com/newsletter/2_2011/IEEE%20Reliability%20Society%20Newsletter.files/Operational%20Implications%20of%20the%20DNS%20Control%20Plane.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=173" title="Zhenkai Zhu, Ryuji Wakikawa, and Lixia Zhang, &lt;strong&gt;&amp;quot;SAIL: A Scalable Approach for Wide-Area IP Mobility&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE INFOCOM Mobiworld Workshop&lt;/em&gt;, April  2011. "><img src="/images/extensions/bib.png" /></a>

     Zhenkai Zhu, Ryuji Wakikawa, and Lixia Zhang, <br/><strong>&quot;SAIL: A Scalable Approach for Wide-Area IP Mobility</strong>,&quot; <br/>in <em>Proceedings of IEEE INFOCOM Mobiworld Workshop</em>, April  2011.

        <a target="_blank" href="http://irl.cs.ucla.edu/~zhenkai/SAIL.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=174" title="Jaeyoung Choi, Jong Han Park, Pei-Chun Cheng, Dorian Kim, and Lixia Zhang, &lt;strong&gt;&amp;quot;Understanding BGP Next-hop Diversity&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE Global Internet Symposium (INFOCOM workshop)&lt;/em&gt;, April  2011, pp. 846&amp;ndash;851. "><img src="/images/extensions/bib.png" /></a>

     Jaeyoung Choi, Jong Han Park, Pei-Chun Cheng, Dorian Kim, and Lixia Zhang, <br/><strong>&quot;Understanding BGP Next-hop Diversity</strong>,&quot; <br/>in <em>Proceedings of IEEE Global Internet Symposium (INFOCOM workshop)</em>, April  2011, pp. 846&ndash;851.

        <a target="_blank" href="http://www.cs.ucla.edu/~jpark/pathdiv.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=172" title="P-C. Cheng, B. Zhang, D. Massey, and L. Zhang, &lt;strong&gt;&amp;quot;Identifying BGP routing table transfers&lt;/strong&gt;,&amp;quot; &lt;em&gt;Computer Networks&lt;/em&gt;, vol. 55, no. 3, February  2011. "><img src="/images/extensions/bib.png" /></a>

     P-C. Cheng, B. Zhang, D. Massey, and L. Zhang, <br/><strong>&quot;Identifying BGP routing table transfers</strong>,&quot; <br/><em>Computer Networks</em>, vol. 55, no. 3, February  2011.

        <a target="_blank" href="http://dx.doi.org/10.1016/j.comnet.2010.09.002"><img src="/images/extensions/html.png"></a>

    </li>

</ul><h3>2010</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=194" title="Jiangzhe Wang, Ryuji Wakikawa, and Lixia Zhang, &lt;strong&gt;&amp;quot;DMND: Collecting data from mobiles using Named Data&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE Vehicular Networking Conference&lt;/em&gt;, December  2010, pp. 49&amp;ndash;56. "><img src="/images/extensions/bib.png" /></a>

     Jiangzhe Wang, Ryuji Wakikawa, and Lixia Zhang, <br/><strong>&quot;DMND: Collecting data from mobiles using Named Data</strong>,&quot; <br/>in <em>Proceedings of IEEE Vehicular Networking Conference</em>, December  2010, pp. 49&ndash;56.

        <a target="_blank" href="http://www.cs.ucla.edu/~lucas/papers/ldc-ndn.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=54" title="Pei-chun Cheng, Jong Han Park, Keyur Patel, and Lixia Zhang, &lt;strong&gt;&amp;quot;Route Flap Damping With Assured Reachability&lt;/strong&gt;,&amp;quot; &lt;em&gt;AINTEC&lt;/em&gt;, November  2010. "><img src="/images/extensions/bib.png" /></a>

     Pei-chun Cheng, Jong Han Park, Keyur Patel, and Lixia Zhang, <br/><strong>&quot;Route Flap Damping With Assured Reachability</strong>,&quot; <br/><em>AINTEC</em>, November  2010.

        <a target="_blank" href="/papers/rfdrg_aintec.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=55" title="Jong Han Park, Dan Jen, Mohit Lad, Shane Amante, Danny McPherson, and Lixia Zhang, &lt;strong&gt;&amp;quot;Investigating Occurrence of Duplicate Updates in BGP Announcements&lt;/strong&gt;,&amp;quot; &lt;em&gt;Passive and Active Measurement&lt;/em&gt;, April  2010. "><img src="/images/extensions/bib.png" /></a>

     Jong Han Park, Dan Jen, Mohit Lad, Shane Amante, Danny McPherson, and Lixia Zhang, <br/><strong>&quot;Investigating Occurrence of Duplicate Updates in BGP Announcements</strong>,&quot; <br/><em>Passive and Active Measurement</em>, April  2010.

        <a target="_blank" href="http://www.cs.ucla.edu/~jpark/dupbgp.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=56" title="Pei-chun Cheng, Xin Zhao, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Longitudinal Study of BGP Monitor Session Failures&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM Computer Communication Review (CCR)&lt;/em&gt;, April  2010. "><img src="/images/extensions/bib.png" /></a>

     Pei-chun Cheng, Xin Zhao, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Longitudinal Study of BGP Monitor Session Failures</strong>,&quot; <br/><em>ACM SIGCOMM Computer Communication Review (CCR)</em>, April  2010.

        <a target="_blank" href="http://www.cs.arizona.edu/~bzhang/paper/10-ccr-reset.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=199" title="Alexander Afanasyev, Neil Tilley, Brent Longstaff, and Lixia Zhang, &lt;strong&gt;&amp;quot;BGP Routing Table: Trends and Challenges&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 12th Youth Technological Conference &amp;quot;High Technologies and Intellectual Systems&amp;quot;&lt;/em&gt;, Moscow, Russia, April  2010. "><img src="/images/extensions/bib.png" /></a>

     Alexander Afanasyev, Neil Tilley, Brent Longstaff, and Lixia Zhang, <br/><strong>&quot;BGP Routing Table: Trends and Challenges</strong>,&quot; <br/>in <em>Proceedings of the 12th Youth Technological Conference &quot;High Technologies and Intellectual Systems&quot;</em>, Moscow, Russia, April  2010.


    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=57" title="Ricardo Oliveira, Dan Pei, Walter Willinger, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;The (in)Completeness of the Observed Internet AS-level Structure&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE/ACM Transactions on Networking&lt;/em&gt;, January  2010. "><img src="/images/extensions/bib.png" /></a>

     Ricardo Oliveira, Dan Pei, Walter Willinger, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;The (in)Completeness of the Observed Internet AS-level Structure</strong>,&quot; <br/><em>IEEE/ACM Transactions on Networking</em>, January  2010.

        <a target="_blank" href="/papers/0completeness.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=193" title="Jiangzhe Wang, Eric Osterweil, Chunyi Peng, Ryuji Wakikawa, Lixia Zhang, Chiyu Li, and Pei-chun Cheng, &lt;strong&gt;&amp;quot;Implementing instant messaging using named data&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the Sixth Asian Internet Engineering Conference&lt;/em&gt;,  2010, pp. 40&amp;ndash;47. "><img src="/images/extensions/bib.png" /></a>

     Jiangzhe Wang, Eric Osterweil, Chunyi Peng, Ryuji Wakikawa, Lixia Zhang, Chiyu Li, and Pei-chun Cheng, <br/><strong>&quot;Implementing instant messaging using named data</strong>,&quot; <br/>in <em>Proceedings of the Sixth Asian Internet Engineering Conference</em>,  2010, pp. 40&ndash;47.

        <a target="_blank" href="http://www.cs.ucla.edu/~lucas/papers/ndnpurple.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2009</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=58" title="Eric Osterweil, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Deploying and Monitoring DNS Security (DNSSEC)&lt;/strong&gt;,&amp;quot; &lt;em&gt;25th Annual Computer Security Applications Conference (ACSAC &#039;09)&lt;/em&gt;, December  2009. "><img src="/images/extensions/bib.png" /></a>

     Eric Osterweil, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Deploying and Monitoring DNS Security (DNSSEC)</strong>,&quot; <br/><em>25th Annual Computer Security Applications Conference (ACSAC '09)</em>, December  2009.

        <a target="_blank" href="/papers/acsac-09.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=59" title="Eric Osterweil and Lixia Zhang, &lt;strong&gt;&amp;quot;Interadministrative  Challenges in   Managing DNSKEYs&lt;/strong&gt;,&amp;quot; &lt;em&gt;Security and Privacy Magazine: Securing the Domain Name System&lt;/em&gt;, September  2009. "><img src="/images/extensions/bib.png" /></a>

     Eric Osterweil and Lixia Zhang, <br/><strong>&quot;Interadministrative  Challenges in   Managing DNSKEYs</strong>,&quot; <br/><em>Security and Privacy Magazine: Securing the Domain Name System</em>, September  2009.

        <a target="_blank" href="/papers/j5ost.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=60" title="Ricardo Oliveira, Mohit Lad, and Lixia Zhang, &lt;strong&gt;&amp;quot;Understanding the Challenges in Securing Internet Routing&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE FIST Workshop&lt;/em&gt;, July  2009. "><img src="/images/extensions/bib.png" /></a>

     Ricardo Oliveira, Mohit Lad, and Lixia Zhang, <br/><strong>&quot;Understanding the Challenges in Securing Internet Routing</strong>,&quot; <br/><em>IEEE FIST Workshop</em>, July  2009.

        <a target="_blank" href="/papers/routesec.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=61" title="Eric Osterweil, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Managing Trusted Keys in Internet-Scale Systems&lt;/strong&gt;,&amp;quot; &lt;em&gt;The First Workshop on Trust and Security in the Future Internet (FIST &#039;09)&lt;/em&gt;, June  2009. "><img src="/images/extensions/bib.png" /></a>

     Eric Osterweil, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Managing Trusted Keys in Internet-Scale Systems</strong>,&quot; <br/><em>The First Workshop on Trust and Security in the Future Internet (FIST '09)</em>, June  2009.

        <a target="_blank" href="/papers/tas-fist09.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=191" title="Lixia Zhang, Ryuji Wakikawa, and Zhenkai Zhu, &lt;strong&gt;&amp;quot;Support mobility in the global internet&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 1st ACM workshop on Mobile internet through cellular networks&lt;/em&gt;,  2009, pp. 1&amp;ndash;6. "><img src="/images/extensions/bib.png" /></a>

     Lixia Zhang, Ryuji Wakikawa, and Zhenkai Zhu, <br/><strong>&quot;Support mobility in the global internet</strong>,&quot; <br/>in <em>Proceedings of the 1st ACM workshop on Mobile internet through cellular networks</em>,  2009, pp. 1&ndash;6.

        <a target="_blank" href="http://www.cs.ucla.edu/~lixia/papers/09MICNET.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2008</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=62" title="Eric Osterweil, Michael Ryan, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Quantifying the Operational Status of the DNSSEC Deployment&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 6th ACM/USENIX Internet Measurement Conference (IMC&#039;08)&lt;/em&gt;, Vouliagmeni, Greece, October  2008. "><img src="/images/extensions/bib.png" /></a>

     Eric Osterweil, Michael Ryan, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Quantifying the Operational Status of the DNSSEC Deployment</strong>,&quot; <br/>in <em>Proceedings of the 6th ACM/USENIX Internet Measurement Conference (IMC'08)</em>, Vouliagmeni, Greece, October  2008.

        <a target="_blank" href="/papers/imc71-osterweil.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=63" title="Dan Jen, Michael Meisel, He Yan, Dan Massey, Lan Wang, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Towards a New Internet Routing Architecture: Arguments for Separating Edges from Transit Core&lt;/strong&gt;,&amp;quot; &lt;em&gt;HotNets-VII&lt;/em&gt;, October  2008. "><img src="/images/extensions/bib.png" /></a>

     Dan Jen, Michael Meisel, He Yan, Dan Massey, Lan Wang, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Towards a New Internet Routing Architecture: Arguments for Separating Edges from Transit Core</strong>,&quot; <br/><em>HotNets-VII</em>, October  2008.

        <a target="_blank" href="http://conferences.sigcomm.org/hotnets/2008/papers/18.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=65" title="Ricardo Oliveira, Dan Pei, Walter Willinger, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;In Search of the elusive Ground Truth: The Internet&#039;s AS-level Connectivity Structure&lt;/strong&gt;,&amp;quot; &lt;em&gt;Sigmetrics&lt;/em&gt;, June  2008. "><img src="/images/extensions/bib.png" /></a>

     Ricardo Oliveira, Dan Pei, Walter Willinger, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;In Search of the elusive Ground Truth: The Internet's AS-level Connectivity Structure</strong>,&quot; <br/><em>Sigmetrics</em>, June  2008.

        <a target="_blank" href="/papers/completeness.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=66" title="Ricardo Oliveira, Beichuan Zhang, Dan Pei, and Lixia Zhang, &lt;strong&gt;&amp;quot;Quantifying Path Exploration in the Internet&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM/IEEE Transactions on Networking&lt;/em&gt;, June  2008. "><img src="/images/extensions/bib.png" /></a>

     Ricardo Oliveira, Beichuan Zhang, Dan Pei, and Lixia Zhang, <br/><strong>&quot;Quantifying Path Exploration in the Internet</strong>,&quot; <br/><em>ACM/IEEE Transactions on Networking</em>, June  2008.

        <a target="_blank" href="/papers/pathrank-ton.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2007</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=67" title="Eric Osterweil, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Observations from the DNSSEC Deployment&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE ICNP Workshop on Secure Network Protocols (NPSec)&lt;/em&gt;, October  2007. "><img src="/images/extensions/bib.png" /></a>

     Eric Osterweil, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Observations from the DNSSEC Deployment</strong>,&quot; <br/>in <em>Proceedings of IEEE ICNP Workshop on Secure Network Protocols (NPSec)</em>, October  2007.

        <a target="_blank" href="/papers/SecSpider_NPSec07.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=68" title="Ricardo Oliveira, Mohit Lad, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Geographically Informed Inter-Domain Routing&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE ICNP&lt;/em&gt;, Beijing, China, October  2007. "><img src="/images/extensions/bib.png" /></a>

     Ricardo Oliveira, Mohit Lad, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Geographically Informed Inter-Domain Routing</strong>,&quot; <br/>in <em>Proceedings of IEEE ICNP</em>, Beijing, China, October  2007.

        <a target="_blank" href="/papers/giro.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=69" title="Mohit Lad, Ricardo Oliveira, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Inferring the Origin of Routing Changes using Link Weights&lt;/strong&gt;,&amp;quot; in &lt;em&gt;IEEE ICNP&lt;/em&gt;, Beijing, China, October  2007. "><img src="/images/extensions/bib.png" /></a>

     Mohit Lad, Ricardo Oliveira, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Inferring the Origin of Routing Changes using Link Weights</strong>,&quot; <br/>in <em>IEEE ICNP</em>, Beijing, China, October  2007.

        <a target="_blank" href="/papers/mlad-InferringOrigin.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=70" title="Eric Osterweil, Vasileios Pappas, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Zone State Revocation for DNSSEC&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM Workshop on Large-Scale Attack Defense (LSAD)&lt;/em&gt;, August  2007. "><img src="/images/extensions/bib.png" /></a>

     Eric Osterweil, Vasileios Pappas, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Zone State Revocation for DNSSEC</strong>,&quot; <br/><em>ACM SIGCOMM Workshop on Large-Scale Attack Defense (LSAD)</em>, August  2007.

        <a target="_blank" href="/papers/zsr-lsad07.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=71" title="Ricardo Oliveira, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Observing the Evolution of Internet AS Topology&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM&lt;/em&gt;, August  2007. "><img src="/images/extensions/bib.png" /></a>

     Ricardo Oliveira, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Observing the Evolution of Internet AS Topology</strong>,&quot; <br/><em>ACM SIGCOMM</em>, August  2007.

        <a target="_blank" href="/papers/fp163_oliveira.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=72" title="Dan Massey, Lan Wang, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Scalable Routing System Design for Future Internet&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM Workshop on IPv6&lt;/em&gt;, August  2007. "><img src="/images/extensions/bib.png" /></a>

     Dan Massey, Lan Wang, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;A Scalable Routing System Design for Future Internet</strong>,&quot; <br/><em>ACM SIGCOMM Workshop on IPv6</em>, August  2007.

        <a target="_blank" href="http://www.cs.ucla.edu/~lixia/papers/07SIG_IP6WS.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=73" title="Ricardo Oliveira, Mohit Lad, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Geographically Informed Inter-Domain Routing&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM poster session&lt;/em&gt;, August  2007. "><img src="/images/extensions/bib.png" /></a>

     Ricardo Oliveira, Mohit Lad, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Geographically Informed Inter-Domain Routing</strong>,&quot; <br/><em>ACM SIGCOMM poster session</em>, August  2007.

        <a target="_blank" href="http://www.cs.ucla.edu/~lixia/papers/07SIGPoster_giro.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=74" title="Ricardo Oliveira, Ying-Ju Chi, Yannis Pefkianakis, Mohit Lad, and Lixia Zhang, &lt;strong&gt;&amp;quot;Visualizing  Internet Topology Dynamics with Cyclops&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM poster session&lt;/em&gt;, August  2007. "><img src="/images/extensions/bib.png" /></a>

     Ricardo Oliveira, Ying-Ju Chi, Yannis Pefkianakis, Mohit Lad, and Lixia Zhang, <br/><strong>&quot;Visualizing  Internet Topology Dynamics with Cyclops</strong>,&quot; <br/><em>ACM SIGCOMM poster session</em>, August  2007.

        <a target="_blank" href="http://www.cs.ucla.edu/~lixia/papers/07SIGPoster_cyclops.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=75" title="Mohit Lad, Ricardo Oliveira, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Understanding the Resiliency of Internet Topology against Prefix Hijack Attacks&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE/IFIP Dependable Systems and Networks (DSN)&lt;/em&gt;, June  2007. "><img src="/images/extensions/bib.png" /></a>

     Mohit Lad, Ricardo Oliveira, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Understanding the Resiliency of Internet Topology against Prefix Hijack Attacks</strong>,&quot; <br/><em>IEEE/IFIP Dependable Systems and Networks (DSN)</em>, June  2007.

        <a target="_blank" href="/papers/hijack-dsn.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=76" title="Arnaud Legout, Nikitas Liogkas, Eddie Kohler, , and Lixia Zhang, &lt;strong&gt;&amp;quot;Clustering and Sharing Incentives in BitTorrent Systems&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGMETRICS 2007, San Diego, CA&lt;/em&gt;, June  2007. "><img src="/images/extensions/bib.png" /></a>

     Arnaud Legout, Nikitas Liogkas, Eddie Kohler, , and Lixia Zhang, <br/><strong>&quot;Clustering and Sharing Incentives in BitTorrent Systems</strong>,&quot; <br/><em>ACM SIGMETRICS 2007, San Diego, CA</em>, June  2007.

        <a target="_blank" href="http://hal.inria.fr/inria-00137444/en/"><img src="/images/extensions/html.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=77" title="Vasilis Pappas, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Enhancing DNS Resilience against Denial of Service Attacks&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE/IFIP Dependable Systems and Networks (DSN)&lt;/em&gt;, June  2007. "><img src="/images/extensions/bib.png" /></a>

     Vasilis Pappas, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Enhancing DNS Resilience against Denial of Service Attacks</strong>,&quot; <br/><em>IEEE/IFIP Dependable Systems and Networks (DSN)</em>, June  2007.

        <a target="_blank" href="http://www.cs.ucla.edu/~lixia/papers/07DSN_TTL.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2006</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=78" title="Mohit Lad, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Visualizing Internet routing changes&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Transactions on Visualization and Computer Graphics&lt;/em&gt;, November  2006. "><img src="/images/extensions/bib.png" /></a>

     Mohit Lad, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Visualizing Internet routing changes</strong>,&quot; <br/><em>IEEE Transactions on Visualization and Computer Graphics</em>, November  2006.

        <a target="_blank" href="http://www.cs.ucla.edu/~mohit/research.html#publications"><img src="/images/extensions/html.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=79" title="Ricardo Oliveira, Beichuan Zhang, Dan Pei, Rafit Izhak-Ratzin, and Lixia Zhang, &lt;strong&gt;&amp;quot;Quantifying Path Exploration in the Internet&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM/USENIX Internet Measurement Conference (IMC), Rio de Janeiro, Brazil.&lt;/em&gt; October  2006. "><img src="/images/extensions/bib.png" /></a>

     Ricardo Oliveira, Beichuan Zhang, Dan Pei, Rafit Izhak-Ratzin, and Lixia Zhang, <br/><strong>&quot;Quantifying Path Exploration in the Internet</strong>,&quot; <br/><em>ACM SIGCOMM/USENIX Internet Measurement Conference (IMC), Rio de Janeiro, Brazil.</em> October  2006.

        <a target="_blank" href="/papers/imc175f-oliveira.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=80" title="Mohit Lad, Dan Massey, Adam Meyerson, Akash Nanavati, , and Lixia Zhang, &lt;strong&gt;&amp;quot;Minimum failure explanations for path vector routing changes&lt;/strong&gt;,&amp;quot; &lt;em&gt;Journal of Combinatorial optimization&lt;/em&gt;, September  2006. "><img src="/images/extensions/bib.png" /></a>

     Mohit Lad, Dan Massey, Adam Meyerson, Akash Nanavati, , and Lixia Zhang, <br/><strong>&quot;Minimum failure explanations for path vector routing changes</strong>,&quot; <br/><em>Journal of Combinatorial optimization</em>, September  2006.

        <a target="_blank" href="/papers/Joco_Final_minFault.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=81" title="Mohit Lad, Dan Massey, Dan Pei, Yiguo Wu, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;PHAS: a prefix hijack alert system&lt;/strong&gt;,&amp;quot; &lt;em&gt;USENIX Security&lt;/em&gt;, August  2006. "><img src="/images/extensions/bib.png" /></a>

     Mohit Lad, Dan Massey, Dan Pei, Yiguo Wu, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;PHAS: a prefix hijack alert system</strong>,&quot; <br/><em>USENIX Security</em>, August  2006.

        <a target="_blank" href="/papers/originChange.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=82" title="Eric Osterweil, Dan Massey, Batsukh Tsendjav, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Security Through Publicity&lt;/strong&gt;,&amp;quot; &lt;em&gt;USENIX Security, HotSec&lt;/em&gt;, July  2006. "><img src="/images/extensions/bib.png" /></a>

     Eric Osterweil, Dan Massey, Batsukh Tsendjav, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Security Through Publicity</strong>,&quot; <br/><em>USENIX Security, HotSec</em>, July  2006.

        <a target="_blank" href="/papers/pski.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=83" title="Beichuan Zhang, Wenjie Wang, Sugih Jamin, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Universal IP Multicast Delivery&lt;/strong&gt;,&amp;quot; &lt;em&gt;The special issue of Computer Networks on Overlay Distribution Structures and their Applications&lt;/em&gt;, April  2006. "><img src="/images/extensions/bib.png" /></a>

     Beichuan Zhang, Wenjie Wang, Sugih Jamin, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Universal IP Multicast Delivery</strong>,&quot; <br/><em>The special issue of Computer Networks on Overlay Distribution Structures and their Applications</em>, April  2006.

        <a target="_blank" href="http://www.cs.arizona.edu/people/bzhang/paper/umcast.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=84" title="Vasileios Pappas, Daniel Massey, Andreas Terzis, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Comparative Study of Current DNS with DHT-Based Alternatives&lt;/strong&gt;,&amp;quot; &lt;em&gt;INFOCOM&lt;/em&gt;, April  2006. "><img src="/images/extensions/bib.png" /></a>

     Vasileios Pappas, Daniel Massey, Andreas Terzis, and Lixia Zhang, <br/><strong>&quot;A Comparative Study of Current DNS with DHT-Based Alternatives</strong>,&quot; <br/><em>INFOCOM</em>, April  2006.

        <a target="_blank" href="/papers/vp_inf06.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=85" title="H. Yang, S. Lu, F. Ricciato, and L. Zhang, &lt;strong&gt;&amp;quot;Securing a Wireless World&lt;/strong&gt;,&amp;quot; &lt;em&gt;The Proceedings of IEEE Special Issue on Security and Cryptography&lt;/em&gt;, February  2006. "><img src="/images/extensions/bib.png" /></a>

     H. Yang, S. Lu, F. Ricciato, and L. Zhang, <br/><strong>&quot;Securing a Wireless World</strong>,&quot; <br/><em>The Proceedings of IEEE Special Issue on Security and Cryptography</em>, February  2006.

        <a target="_blank" href="/papers/ProcIEEE.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=86" title="Nikitas Liogkas, Rober t Nelson, Eddie Kohler, , and Lixia Zhang, &lt;strong&gt;&amp;quot;Exploiting BitTorrent For Fun (But Not Profit)&lt;/strong&gt;,&amp;quot; &lt;em&gt;The 5th International Workshop on Peer-to-Peer Systems (IPTPS)&lt;/em&gt;, February  2006. "><img src="/images/extensions/bib.png" /></a>

     Nikitas Liogkas, Rober t Nelson, Eddie Kohler, , and Lixia Zhang, <br/><strong>&quot;Exploiting BitTorrent For Fun (But Not Profit)</strong>,&quot; <br/><em>The 5th International Workshop on Peer-to-Peer Systems (IPTPS)</em>, February  2006.

        <a target="_blank" href="/data/files/papers/Liogkas-BitTorrent06.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=87" title="Dan Pei, Beichuan Zhang, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;An Analysis of Convergence Delay in Path Vector Routing Protocols&lt;/strong&gt;,&amp;quot; &lt;em&gt;Computer Networks, Volume 50, Issue 3&lt;/em&gt;, February  2006. "><img src="/images/extensions/bib.png" /></a>

     Dan Pei, Beichuan Zhang, Dan Massey, and Lixia Zhang, <br/><strong>&quot;An Analysis of Convergence Delay in Path Vector Routing Protocols</strong>,&quot; <br/><em>Computer Networks, Volume 50, Issue 3</em>, February  2006.

        <a target="_blank" href="/papers/convergence.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2005</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=88" title="Ricardo V. Oliveira, Rafit Izhak-Ratzin, Beichuan Zhang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Measurement of Highly Active Prefixes in BGP&lt;/strong&gt;,&amp;quot; &lt;em&gt;In GLOBECOM&lt;/em&gt;, November  2005. "><img src="/images/extensions/bib.png" /></a>

     Ricardo V. Oliveira, Rafit Izhak-Ratzin, Beichuan Zhang, and Lixia Zhang, <br/><strong>&quot;Measurement of Highly Active Prefixes in BGP</strong>,&quot; <br/><em>In GLOBECOM</em>, November  2005.

        <a target="_blank" href="/papers/activity.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=89" title="Hyo-Joeng Shin, Dan Pei, Mohit Lad, Yanghee Choi, , and Lixia Zhang, &lt;strong&gt;&amp;quot;The Impact of Multi-homing on Network Reliability and Stability: A Case Study&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE ICCCN&lt;/em&gt;, October  2005. "><img src="/images/extensions/bib.png" /></a>

     Hyo-Joeng Shin, Dan Pei, Mohit Lad, Yanghee Choi, , and Lixia Zhang, <br/><strong>&quot;The Impact of Multi-homing on Network Reliability and Stability: A Case Study</strong>,&quot; <br/><em>IEEE ICCCN</em>, October  2005.

        <a target="_blank" href="/papers/imh.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=90" title="Beichuan Zhang, Vamsi Kambhampati, Mohit Lad, Daniel Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Identifying  BGP Routing Table Transfers&lt;/strong&gt;,&amp;quot; &lt;em&gt;SIGCOMM Mining the Network Data (MineNet) Workshop&lt;/em&gt;, August  2005. "><img src="/images/extensions/bib.png" /></a>

     Beichuan Zhang, Vamsi Kambhampati, Mohit Lad, Daniel Massey, and Lixia Zhang, <br/><strong>&quot;Identifying  BGP Routing Table Transfers</strong>,&quot; <br/><em>SIGCOMM Mining the Network Data (MineNet) Workshop</em>, August  2005.

        <a target="_blank" href="/papers/05-minenet-mct.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=91" title="D. Clark, C. Partridge, R. Braden, B. Davie, S. Floyd, V. Jacobson, D. Katabi, G. Minshall, K. K. Ramakrishnan, T. Roscoe, I. Stoica, J. Wroclawski, , and L. Zhang, &lt;strong&gt;&amp;quot;Making the World (of Communications) a Different Place&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACMComputer Communication Review,Vol. 35, No. 3, pp. 91-96&lt;/em&gt;, July  2005. "><img src="/images/extensions/bib.png" /></a>

     D. Clark, C. Partridge, R. Braden, B. Davie, S. Floyd, V. Jacobson, D. Katabi, G. Minshall, K. K. Ramakrishnan, T. Roscoe, I. Stoica, J. Wroclawski, , and L. Zhang, <br/><strong>&quot;Making the World (of Communications) a Different Place</strong>,&quot; <br/><em>ACMComputer Communication Review,Vol. 35, No. 3, pp. 91-96</em>, July  2005.

        <a target="_blank" href="/papers/e2e-vision.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=92" title="Beichuan Zhang, Dan Pei, Daniel Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Timer Interaction in Route Flap Damping&lt;/strong&gt;,&amp;quot; &lt;em&gt;The 25th International Conference on Distributed Computing Systems (ICDCS)&lt;/em&gt;, June  2005. "><img src="/images/extensions/bib.png" /></a>

     Beichuan Zhang, Dan Pei, Daniel Massey, and Lixia Zhang, <br/><strong>&quot;Timer Interaction in Route Flap Damping</strong>,&quot; <br/><em>The 25th International Conference on Distributed Computing Systems (ICDCS)</em>, June  2005.

        <a target="_blank" href="http://www.cs.ucla.edu/~bzhang/paper/dtimer.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=93" title="Dan Pei, Matt Azuma, Daniel Massey, , and Lixia Zhang, &lt;strong&gt;&amp;quot;BGP-RCN: Improving BGP Convergence Through Root Cause Notification&lt;/strong&gt;,&amp;quot; &lt;em&gt;Computer Networks, Volume 48, Issue 2, Pages 175-194&lt;/em&gt;, June  2005. "><img src="/images/extensions/bib.png" /></a>

     Dan Pei, Matt Azuma, Daniel Massey, , and Lixia Zhang, <br/><strong>&quot;BGP-RCN: Improving BGP Convergence Through Root Cause Notification</strong>,&quot; <br/><em>Computer Networks, Volume 48, Issue 2, Pages 175-194</em>, June  2005.

        <a target="_blank" href="/papers/massey_comnet05.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=94" title="Fan Ye, Haiyun Luo, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;Statistical En-Route Filtering in Wireless Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Jounal on Selected Areas in Communications, Special Issue on Self-organizing Distributed Collaborative Sensor Networks, Vol. 23, No. 4, pp. 839-850&lt;/em&gt;, April  2005. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Haiyun Luo, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;Statistical En-Route Filtering in Wireless Sensor Networks</strong>,&quot; <br/><em>IEEE Jounal on Selected Areas in Communications, Special Issue on Self-organizing Distributed Collaborative Sensor Networks, Vol. 23, No. 4, pp. 839-850</em>, April  2005.

        <a target="_blank" href="/papers/sef-jsac.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=95" title="Xiaoliang Zhao, Beichuan Zhang, Andreas Terzis, Daniel Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;The Impact of Link Failure Location on Routing Dynamics: A Formal Analysis&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM Asia Workshop&lt;/em&gt;, April  2005. "><img src="/images/extensions/bib.png" /></a>

     Xiaoliang Zhao, Beichuan Zhang, Andreas Terzis, Daniel Massey, and Lixia Zhang, <br/><strong>&quot;The Impact of Link Failure Location on Routing Dynamics: A Formal Analysis</strong>,&quot; <br/><em>ACM SIGCOMM Asia Workshop</em>, April  2005.

        <a target="_blank" href="/papers/05-asia-location.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=96" title="Zhenghua Fu, Haiyun Luo, Petros Zerfos, Songwu Lu, Lixia Zhang, and Mario Gerla, &lt;strong&gt;&amp;quot;The Impact of Multihop Wireless Channel on TCP Performance&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Transactions on Mobile Computing, Vol. 4, No. 2, pp. 209-221&lt;/em&gt;, March  2005. "><img src="/images/extensions/bib.png" /></a>

     Zhenghua Fu, Haiyun Luo, Petros Zerfos, Songwu Lu, Lixia Zhang, and Mario Gerla, <br/><strong>&quot;The Impact of Multihop Wireless Channel on TCP Performance</strong>,&quot; <br/><em>IEEE Transactions on Mobile Computing, Vol. 4, No. 2, pp. 209-221</em>, March  2005.

        <a target="_blank" href="http://www.cs.ucla.edu/wing/publication/papers/Fu.TMC04.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=97" title="Fan Ye, Gary Zhong, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;GRAdient Broadcast: A robust Data Delivery Protocol for Large Scale Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM Wireless Networks (WINET) Journal, Vol. 11, No.2&lt;/em&gt;, March  2005. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Gary Zhong, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;GRAdient Broadcast: A robust Data Delivery Protocol for Large Scale Sensor Networks</strong>,&quot; <br/><em>ACM Wireless Networks (WINET) Journal, Vol. 11, No.2</em>, March  2005.

        <a target="_blank" href="/papers/grab-winet.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=98" title="Haiyun Luo, Fan Ye, Jerry Cheng, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;TTDD: Two-Tier Data Dissemination in Large-scale Wireless Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM Wireless Networks, Vol. 11, Issue 1-2, pp. 161-175,&lt;/em&gt; January  2005. "><img src="/images/extensions/bib.png" /></a>

     Haiyun Luo, Fan Ye, Jerry Cheng, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;TTDD: Two-Tier Data Dissemination in Large-scale Wireless Sensor Networks</strong>,&quot; <br/><em>ACM Wireless Networks, Vol. 11, Issue 1-2, pp. 161-175,</em> January  2005.

        <a target="_blank" href="http://www-faculty.cs.uiuc.edu/~haiyun/publications/WINET05.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=99" title="Beichuan Zhang, Raymond Liu, Daniel Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Collecting the Internet AS-level Topology&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM Computer Communication Review (CCR) special issue on Internet Vital Statistics&lt;/em&gt;, January  2005. "><img src="/images/extensions/bib.png" /></a>

     Beichuan Zhang, Raymond Liu, Daniel Massey, and Lixia Zhang, <br/><strong>&quot;Collecting the Internet AS-level Topology</strong>,&quot; <br/><em>ACM SIGCOMM Computer Communication Review (CCR) special issue on Internet Vital Statistics</em>, January  2005.

        <a target="_blank" href="/papers/05-ccr-topology.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=100" title="Xiaoqiao Meng, Zhiguo Xu, Beichuan Zhang, Geoff Huston, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;IPv4 Address Allocation and BGP Routing Table Evolution&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SIGCOMM Computer Communication Review (CCR) special issue on Internet Vital Statistics&lt;/em&gt;, January  2005. "><img src="/images/extensions/bib.png" /></a>

     Xiaoqiao Meng, Zhiguo Xu, Beichuan Zhang, Geoff Huston, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;IPv4 Address Allocation and BGP Routing Table Evolution</strong>,&quot; <br/><em>ACM SIGCOMM Computer Communication Review (CCR) special issue on Internet Vital Statistics</em>, January  2005.

        <a target="_blank" href="/papers/05-ccr-address.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=101" title="Fan Ye, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Randomized Energy-Conservation Protocol for Resilient Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM Wireless Networks&lt;/em&gt;, January  2005. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;A Randomized Energy-Conservation Protocol for Resilient Sensor Networks</strong>,&quot; <br/><em>ACM Wireless Networks</em>, January  2005.

        <a target="_blank" href="/papers/peas-winet.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2004</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=102" title="Haiyun Luo, Jiejun Kong, Petros Zerfos, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;URSA: Ubiquitous and Robust Access Control for Mobile Ad-Hoc Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE/ACM Transactions on Networking (pp1049-1063)&lt;/em&gt;, December  2004. "><img src="/images/extensions/bib.png" /></a>

     Haiyun Luo, Jiejun Kong, Petros Zerfos, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;URSA: Ubiquitous and Robust Access Control for Mobile Ad-Hoc Networks</strong>,&quot; <br/><em>IEEE/ACM Transactions on Networking (pp1049-1063)</em>, December  2004.

        <a target="_blank" href="/papers/Luo.TON04.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=103" title="V. Pappas, Z. Xu, S. Lu, D. Massey, A. Terzis, and L. Zhang, &lt;strong&gt;&amp;quot;Impact of Configuration Errors on DNS Robustness&amp;quot;&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of ACM SIGCOMM&lt;/em&gt;, August  2004. "><img src="/images/extensions/bib.png" /></a>

     V. Pappas, Z. Xu, S. Lu, D. Massey, A. Terzis, and L. Zhang, <br/><strong>&quot;Impact of Configuration Errors on DNS Robustness&quot;</strong>,&quot; <br/>in <em>Proceedings of ACM SIGCOMM</em>, August  2004.

        <a target="_blank" href="/papers/vp_sigcomm04.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=104" title="V. Pappas, P.Faltstrom, D. Massey, and L. Zhang, &lt;strong&gt;&amp;quot;Distributed DNS Troubleshooting&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of ACM SIGCOMM Network Troubleshooting Workshop&lt;/em&gt;, August  2004. "><img src="/images/extensions/bib.png" /></a>

     V. Pappas, P.Faltstrom, D. Massey, and L. Zhang, <br/><strong>&quot;Distributed DNS Troubleshooting</strong>,&quot; <br/>in <em>Proceedings of ACM SIGCOMM Network Troubleshooting Workshop</em>, August  2004.

        <a target="_blank" href="/papers/vp_nts04.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=105" title="Fan Ye, Haiyun Luo, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;Statistical En-route Detection and Filtering of Injected False Data in Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE INFOCOM&lt;/em&gt;, August  2004. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Haiyun Luo, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;Statistical En-route Detection and Filtering of Injected False Data in Sensor Networks</strong>,&quot; <br/><em>IEEE INFOCOM</em>, August  2004.

        <a target="_blank" href="/papers/fan_sef_infocom04.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=106" title="Yuval Shavitt, Dan Raz, and Lixia Zhang, &lt;strong&gt;&amp;quot;Distributed Council Election&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE/ACM Transactions on Networking, 12 (3):483-492&lt;/em&gt;, June  2004. "><img src="/images/extensions/bib.png" /></a>

     Yuval Shavitt, Dan Raz, and Lixia Zhang, <br/><strong>&quot;Distributed Council Election</strong>,&quot; <br/><em>IEEE/ACM Transactions on Networking, 12 (3):483-492</em>, June  2004.

        <a target="_blank" href="/papers/dce-2004-06.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=107" title="Hao Yang, Haiyun Luo, Yang Yi, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;HOURS: Achieving DoS Resilience in an Open Service Hierarchy&lt;/strong&gt;,&amp;quot; &lt;em&gt;The International Conference on Dependable Systems and Networks (DSN), Florence, Italy&lt;/em&gt;, June  2004. "><img src="/images/extensions/bib.png" /></a>

     Hao Yang, Haiyun Luo, Yang Yi, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;HOURS: Achieving DoS Resilience in an Open Service Hierarchy</strong>,&quot; <br/><em>The International Conference on Dependable Systems and Networks (DSN), Florence, Italy</em>, June  2004.

        <a target="_blank" href="/papers/DSN04.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=108" title="Dan Pei, Dan Massey, , and Lixia Zhang, &lt;strong&gt;&amp;quot;A Framework for Resilient Internet Routing Protocols&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Network special issue on Protection, Restoration, and Disaster Recovery&lt;/em&gt;, April  2004. "><img src="/images/extensions/bib.png" /></a>

     Dan Pei, Dan Massey, , and Lixia Zhang, <br/><strong>&quot;A Framework for Resilient Internet Routing Protocols</strong>,&quot; <br/><em>IEEE Network special issue on Protection, Restoration, and Disaster Recovery</em>, April  2004.

        <a target="_blank" href="http://www.cs.ucla.edu/%7Epeidan/network-resilient.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=109" title="Lan Wang, Xiaoliang Zhao, Dan Pei, Randy Bush, Dan Massey, , and Lixia Zhang, &lt;strong&gt;&amp;quot;Protecting BGP Routes to Top Level DNS Servers&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Transactions on Parallel and Distributed Systems&lt;/em&gt;, April  2004. "><img src="/images/extensions/bib.png" /></a>

     Lan Wang, Xiaoliang Zhao, Dan Pei, Randy Bush, Dan Massey, , and Lixia Zhang, <br/><strong>&quot;Protecting BGP Routes to Top Level DNS Servers</strong>,&quot; <br/><em>IEEE Transactions on Parallel and Distributed Systems</em>, April  2004.

        <a target="_blank" href="http://www.cs.ucla.edu/~lixia/papers/03TPDS.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=110" title="Dan Pei, Matt Azuma, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;BGP-RCN: Improving BGP Convergence Through Root Cause Notification&lt;/strong&gt;,&amp;quot; &lt;em&gt;Computer Networks&lt;/em&gt;, April  2004. "><img src="/images/extensions/bib.png" /></a>

     Dan Pei, Matt Azuma, Dan Massey, and Lixia Zhang, <br/><strong>&quot;BGP-RCN: Improving BGP Convergence Through Root Cause Notification</strong>,&quot; <br/><em>Computer Networks</em>, April  2004.

        <a target="_blank" href="/data/files/papers/BGP-RCN.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=111" title="B. Zhang, D. Massey, and L. Zhang, &lt;strong&gt;&amp;quot;Destination Reachability and BGP Convergence Time&lt;/strong&gt;,&amp;quot; &lt;em&gt;GLOBECOM&lt;/em&gt;, April  2004. "><img src="/images/extensions/bib.png" /></a>

     B. Zhang, D. Massey, and L. Zhang, <br/><strong>&quot;Destination Reachability and BGP Convergence Time</strong>,&quot; <br/><em>GLOBECOM</em>, April  2004.

        <a target="_blank" href="/papers/PID43182.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=112" title="Lan Wang, Dan Massey, Keyur Patel, and Lixia Zhang, &lt;strong&gt;&amp;quot;FRTR: A Scalable Mechanism to Restore Routing Table Consistency&lt;/strong&gt;,&amp;quot; &lt;em&gt;DSN&lt;/em&gt;, April  2004. "><img src="/images/extensions/bib.png" /></a>

     Lan Wang, Dan Massey, Keyur Patel, and Lixia Zhang, <br/><strong>&quot;FRTR: A Scalable Mechanism to Restore Routing Table Consistency</strong>,&quot; <br/><em>DSN</em>, April  2004.

        <a target="_blank" href="/papers/frtr.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=113" title="Mohit Lad, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Link-Rank: A Graphical Tool for Capturing Routing Dynamics&lt;/strong&gt;,&amp;quot; &lt;em&gt;Proceedings of The IEEE/IPIF Network Operations and Management Symposium (NOMS)&lt;/em&gt;, April  2004. "><img src="/images/extensions/bib.png" /></a>

     Mohit Lad, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Link-Rank: A Graphical Tool for Capturing Routing Dynamics</strong>,&quot; <br/><em>Proceedings of The IEEE/IPIF Network Operations and Management Symposium (NOMS)</em>, April  2004.

        <a target="_blank" href="/papers/LinkRank.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=114" title="V. Pappas, B. Zhang, A. Terzis, and L. Zhang, &lt;strong&gt;&amp;quot;Fault-Tolerant Data Delivery for Multicast Overlay Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;24th IEEE International Conference on Distributed Computing Systems (ICDCS)&lt;/em&gt;, March  2004. "><img src="/images/extensions/bib.png" /></a>

     V. Pappas, B. Zhang, A. Terzis, and L. Zhang, <br/><strong>&quot;Fault-Tolerant Data Delivery for Multicast Overlay Networks</strong>,&quot; <br/><em>24th IEEE International Conference on Distributed Computing Systems (ICDCS)</em>, March  2004.

        <a target="_blank" href="/papers/vp_icdcs04.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=115" title="Dan Pei, Xiaoliang Zhao, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Study of of BGP Path Vector Route Looping Behavior&lt;/strong&gt;,&amp;quot; &lt;em&gt;24th International Conference On Distributed Computing Systems (ICDCS)&lt;/em&gt;, March  2004. "><img src="/images/extensions/bib.png" /></a>

     Dan Pei, Xiaoliang Zhao, Dan Massey, and Lixia Zhang, <br/><strong>&quot;A Study of of BGP Path Vector Route Looping Behavior</strong>,&quot; <br/><em>24th International Conference On Distributed Computing Systems (ICDCS)</em>, March  2004.

        <a target="_blank" href="/data/files/papers/massey_icdcs04.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=116" title="Mohit Lad, Akash Nanavati, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;An Algorithmic Approach to Identifying Link Failures&lt;/strong&gt;,&amp;quot; &lt;em&gt;Proceedings of the 10th Pacific Rim International Symposium on Dependable Computing (PRDC)&lt;/em&gt;, March  2004. "><img src="/images/extensions/bib.png" /></a>

     Mohit Lad, Akash Nanavati, Dan Massey, and Lixia Zhang, <br/><strong>&quot;An Algorithmic Approach to Identifying Link Failures</strong>,&quot; <br/><em>Proceedings of the 10th Pacific Rim International Symposium on Dependable Computing (PRDC)</em>, March  2004.

        <a target="_blank" href="/papers/LRFault.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=117" title="Hao Yang, Haiyun Luo, Fan Ye, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;Security in Mobile Ad-Hoc Wireless Networks: Challenges and Solutions&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Wireless Communication, Vol. 11, No. 1, pp. 38-47&lt;/em&gt;, February  2004. "><img src="/images/extensions/bib.png" /></a>

     Hao Yang, Haiyun Luo, Fan Ye, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;Security in Mobile Ad-Hoc Wireless Networks: Challenges and Solutions</strong>,&quot; <br/><em>IEEE Wireless Communication, Vol. 11, No. 1, pp. 38-47</em>, February  2004.

        <a target="_blank" href="/papers/WIRELESSCOMM04.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=118" title="Ke Zhang, Felix Wu, Amy Yen, Zhao, Massey, and Zhang, &lt;strong&gt;&amp;quot;On Detection of Anomalous Routing Dynamics in BGP&lt;/strong&gt;,&amp;quot; &lt;em&gt;Networking&lt;/em&gt;, January  2004. "><img src="/images/extensions/bib.png" /></a>

     Ke Zhang, Felix Wu, Amy Yen, Zhao, Massey, and Zhang, <br/><strong>&quot;On Detection of Anomalous Routing Dynamics in BGP</strong>,&quot; <br/><em>Networking</em>, January  2004.

        <a target="_blank" href="/papers/networking04.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>

</ul><h3>2003</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=119" title="Dan Pei, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Detection of Invalid Routing Announcements in the RIP Protocol&lt;/strong&gt;,&amp;quot; &lt;em&gt;GLOBECOM&lt;/em&gt;, December  2003. "><img src="/images/extensions/bib.png" /></a>

     Dan Pei, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Detection of Invalid Routing Announcements in the RIP Protocol</strong>,&quot; <br/><em>GLOBECOM</em>, December  2003.

        <a target="_blank" href="/papers/dan_detection_globalcom03.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=120" title="Mohit Lad, Xiaoliang Zhao, Beichuan Zhang, Dan Massey, and Lixia Zhang, &lt;strong&gt;&amp;quot;Analysis of BGP Update Burst during Slammer Attack&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 5th International Workshop on Distributed Computing&lt;/em&gt;, December  2003. "><img src="/images/extensions/bib.png" /></a>

     Mohit Lad, Xiaoliang Zhao, Beichuan Zhang, Dan Massey, and Lixia Zhang, <br/><strong>&quot;Analysis of BGP Update Burst during Slammer Attack</strong>,&quot; <br/>in <em>Proceedings of the 5th International Workshop on Distributed Computing</em>, December  2003.

        <a target="_blank" href="/papers/mohit_iwdc03.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=121" title="Fan Ye, Haiyun Luo, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;Poster Abstract: Statistical En-route Filtering of Injected False Data In Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM SenSys&lt;/em&gt;, November  2003. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Haiyun Luo, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;Poster Abstract: Statistical En-route Filtering of Injected False Data In Sensor Networks</strong>,&quot; <br/><em>ACM SenSys</em>, November  2003.

        <a target="_blank" href="/papers/fan_statistical_sensys03.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=123" title="Soon-Tee Teoh, Kwan-Liu Ma, Felix S. Wu, Dan Massey, Xiao-Liang Zhao, Dan Pei, Lan Wang, Lixia Zhang, and Randy Bush, &lt;strong&gt;&amp;quot;Visual-based Anomaly Detection for BGP Origin AS Change (OASC) Events&lt;/strong&gt;,&amp;quot; &lt;em&gt;DSOM&lt;/em&gt;, October  2003. "><img src="/images/extensions/bib.png" /></a>

     Soon-Tee Teoh, Kwan-Liu Ma, Felix S. Wu, Dan Massey, Xiao-Liang Zhao, Dan Pei, Lan Wang, Lixia Zhang, and Randy Bush, <br/><strong>&quot;Visual-based Anomaly Detection for BGP Origin AS Change (OASC) Events</strong>,&quot; <br/><em>DSOM</em>, October  2003.

        <a target="_blank" href="/papers/soontee-visual-dsom03.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=124" title="Xiaoliang Zhao, Dan Massey, Dan Pei, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Study on the Routing Convergence of Latin American Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;SIGCOMM Latin America Networking Workshop&lt;/em&gt;, August  2003. "><img src="/images/extensions/bib.png" /></a>

     Xiaoliang Zhao, Dan Massey, Dan Pei, and Lixia Zhang, <br/><strong>&quot;A Study on the Routing Convergence of Latin American Networks</strong>,&quot; <br/><em>SIGCOMM Latin America Networking Workshop</em>, August  2003.

        <a target="_blank" href="/papers/xiaoliang_study_lanc03.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=125" title="Dan Pei, Lan Wang, Daniel Massey, Felix S. Wu, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Study of Packet Delivery Performance during Routing Convergence&lt;/strong&gt;,&amp;quot; &lt;em&gt;DSN&lt;/em&gt;, June  2003. "><img src="/images/extensions/bib.png" /></a>

     Dan Pei, Lan Wang, Daniel Massey, Felix S. Wu, and Lixia Zhang, <br/><strong>&quot;A Study of Packet Delivery Performance during Routing Convergence</strong>,&quot; <br/><em>DSN</em>, June  2003.

        <a target="_blank" href="/papers/peid_packet_dsn03.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=126" title="Yixin Jin, Beichuan Zhang, Vasileios Pappas, Sugih Jamin, and Lixia Zhang, &lt;strong&gt;&amp;quot;DIP: A Scalable Soft-State Protocol for Large Scale Data Dissemination in IDMaps System&lt;/strong&gt;,&amp;quot; &lt;em&gt;The Eighth IEEE Symposiums on Computers and Communications (ISCC)&lt;/em&gt;, June  2003. "><img src="/images/extensions/bib.png" /></a>

     Yixin Jin, Beichuan Zhang, Vasileios Pappas, Sugih Jamin, and Lixia Zhang, <br/><strong>&quot;DIP: A Scalable Soft-State Protocol for Large Scale Data Dissemination in IDMaps System</strong>,&quot; <br/><em>The Eighth IEEE Symposiums on Computers and Communications (ISCC)</em>, June  2003.

        <a target="_blank" href="/papers/yixin_dip_iscc03.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=127" title="Fan Ye, Gary Zhong, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;PEAS: A Robust Energy Conserving Protocol for Long-lived Sensor  Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;23rd International Conference on Distributed Computing Systems (ICDCS)&lt;/em&gt;, May  2003. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Gary Zhong, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;PEAS: A Robust Energy Conserving Protocol for Long-lived Sensor  Networks</strong>,&quot; <br/><em>23rd International Conference on Distributed Computing Systems (ICDCS)</em>, May  2003.

        <a target="_blank" href="/papers/ye-peas-icdcs03.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=128" title="Lan Wang, Xiaoliang Zhao, Dan Pei, Randy Bush, Dan Massey, Allison Mankin, Felix S. Wu, and Lixia Zhang, &lt;strong&gt;&amp;quot;Protecting BGP Routes to Top Level DNS Servers&lt;/strong&gt;,&amp;quot; &lt;em&gt;3rd International Conference on Distributed Computing Systems (ICDCS)&lt;/em&gt;, May  2003. "><img src="/images/extensions/bib.png" /></a>

     Lan Wang, Xiaoliang Zhao, Dan Pei, Randy Bush, Dan Massey, Allison Mankin, Felix S. Wu, and Lixia Zhang, <br/><strong>&quot;Protecting BGP Routes to Top Level DNS Servers</strong>,&quot; <br/><em>3rd International Conference on Distributed Computing Systems (ICDCS)</em>, May  2003.

        <a target="_blank" href="/papers/lanw-dns-filter-ICDCS-2003.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=129" title="Fan Ye, Gary Zhong, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Robust Data Delivery Protocol for Large Scale Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;The 2nd International Workshop on Information Processing in Sensor Networks (IPSN)&lt;/em&gt;, April  2003. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Gary Zhong, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;A Robust Data Delivery Protocol for Large Scale Sensor Networks</strong>,&quot; <br/><em>The 2nd International Workshop on Information Processing in Sensor Networks (IPSN)</em>, April  2003.

        <a target="_blank" href="/papers/ye-ipsn-03.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=130" title="Zhiguo Xu, Xiaoqiao Meng, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;Impact of IPv4 Address Allocation Practise on BGP Routing Table Growth&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Computer Communication Workshop&lt;/em&gt;, March  2003. "><img src="/images/extensions/bib.png" /></a>

     Zhiguo Xu, Xiaoqiao Meng, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;Impact of IPv4 Address Allocation Practise on BGP Routing Table Growth</strong>,&quot; <br/><em>IEEE Computer Communication Workshop</em>, March  2003.

        <a target="_blank" href="/papers/zhiguo_impact_ccw03.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=131" title="Haiyun Luo, Fan Ye, Jerry Cheng, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Two-tier Data Dissemination Model for Large-scale Wireless Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM MONET&lt;/em&gt;, March  2003. "><img src="/images/extensions/bib.png" /></a>

     Haiyun Luo, Fan Ye, Jerry Cheng, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;A Two-tier Data Dissemination Model for Large-scale Wireless Sensor Networks</strong>,&quot; <br/><em>ACM MONET</em>, March  2003.

        <a target="_blank" href="/papers/ttdd-monet03.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=132" title="Zhenghua Fu, Petros Zerfos, Haiyun Luo, Songwu Lu, Lixia Zhang, and Mario Gerla`, &lt;strong&gt;&amp;quot;The Impact of Multihop Wireless Channel on TCP Throughput and Loss&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE INFOCOM&lt;/em&gt;, March  2003. "><img src="/images/extensions/bib.png" /></a>

     Zhenghua Fu, Petros Zerfos, Haiyun Luo, Songwu Lu, Lixia Zhang, and Mario Gerla`, <br/><strong>&quot;The Impact of Multihop Wireless Channel on TCP Throughput and Loss</strong>,&quot; <br/><em>IEEE INFOCOM</em>, March  2003.

        <a target="_blank" href="http://www.cs.ucla.edu/wing/pdfdocs/infocom03.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=133" title="Xiaoliang Zhao, Dan Massey, Felix S. Wu, Mohit Lad, Dan Pei, Lan Wang, and Lixia Zhang, &lt;strong&gt;&amp;quot;Understanding BGP behavior through a study of DoD prefixes&lt;/strong&gt;,&amp;quot; &lt;em&gt;DISCEX&lt;/em&gt;, February  2003. "><img src="/images/extensions/bib.png" /></a>

     Xiaoliang Zhao, Dan Massey, Felix S. Wu, Mohit Lad, Dan Pei, Lan Wang, and Lixia Zhang, <br/><strong>&quot;Understanding BGP behavior through a study of DoD prefixes</strong>,&quot; <br/><em>DISCEX</em>, February  2003.

        <a target="_blank" href="/papers/fniisc_discex03.ps"><img src="/images/extensions/ps.png"></a>

    </li>

</ul><h3>2002</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=134" title="Fan Ye, Gary Zhong, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;PEAS: A Robust Energy Conserving Protocol for Long-lived Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;a poster in the 10 th IEEE Internation Conference on Network Protocols (ICNP)&lt;/em&gt;, November  2002. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Gary Zhong, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;PEAS: A Robust Energy Conserving Protocol for Long-lived Sensor Networks</strong>,&quot; <br/><em>a poster in the 10 th IEEE Internation Conference on Network Protocols (ICNP)</em>, November  2002.

        <a target="_blank" href="http://www.cs.ucla.edu/%7Eyefan/02icnp-poster.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=135" title="Lan Wang, Xiaoliang Zhao, Dan Pei, Randy Bush, Dan Massey, Allison Mankin, Felix S. Wu, and Lixia Zhang, &lt;strong&gt;&amp;quot;Observation and Analysis of BGP Behavior under Stress&lt;/strong&gt;,&amp;quot; &lt;em&gt;SIGCOMM Internet Measurement Workshop&lt;/em&gt;, November  2002. "><img src="/images/extensions/bib.png" /></a>

     Lan Wang, Xiaoliang Zhao, Dan Pei, Randy Bush, Dan Massey, Allison Mankin, Felix S. Wu, and Lixia Zhang, <br/><strong>&quot;Observation and Analysis of BGP Behavior under Stress</strong>,&quot; <br/><em>SIGCOMM Internet Measurement Workshop</em>, November  2002.

        <a target="_blank" href="/papers/lanw-imw02-bgp.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=136" title="Wenjie Wang, David Helder, Sugih Jamin, , and Lixia Zhang, &lt;strong&gt;&amp;quot;Overlay Optimizations for End-host Multicast&lt;/strong&gt;,&amp;quot; &lt;em&gt;Fourth International Workshop on Networked Group Communication (NGC)&lt;/em&gt;, October  2002. "><img src="/images/extensions/bib.png" /></a>

     Wenjie Wang, David Helder, Sugih Jamin, , and Lixia Zhang, <br/><strong>&quot;Overlay Optimizations for End-host Multicast</strong>,&quot; <br/><em>Fourth International Workshop on Networked Group Communication (NGC)</em>, October  2002.

        <a target="_blank" href="/data/files/papers/tmesh_ngc02.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=137" title="Beichuan Zhang, Sugih Jamin, and Lixia Zhang, &lt;strong&gt;&amp;quot;Universal IP Multicast Delivery&lt;/strong&gt;,&amp;quot; &lt;em&gt;Proceedings of Fourth International Workshop on Networked Group Communication (NGC)&lt;/em&gt;, October  2002. "><img src="/images/extensions/bib.png" /></a>

     Beichuan Zhang, Sugih Jamin, and Lixia Zhang, <br/><strong>&quot;Universal IP Multicast Delivery</strong>,&quot; <br/><em>Proceedings of Fourth International Workshop on Networked Group Communication (NGC)</em>, October  2002.

        <a target="_blank" href="/papers/um_ngc02.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=138" title="Fan Ye, Haiyun Luo, Jerry Cheng, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Two-tier Data Dissemination Model for Large-scale Wireless Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;MobiCom&lt;/em&gt;, September  2002. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Haiyun Luo, Jerry Cheng, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;A Two-tier Data Dissemination Model for Large-scale Wireless Sensor Networks</strong>,&quot; <br/><em>MobiCom</em>, September  2002.

        <a target="_blank" href="/papers/ye-mobicom02.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=139" title="Haiyun Luo, Jiejun Kong, Petros Zerfos, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;Self-securing Ad Hoc Wireless Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE ISCC (IEEE Symposium on Computers and Communications)&lt;/em&gt;, July  2002. "><img src="/images/extensions/bib.png" /></a>

     Haiyun Luo, Jiejun Kong, Petros Zerfos, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;Self-securing Ad Hoc Wireless Networks</strong>,&quot; <br/><em>IEEE ISCC (IEEE Symposium on Computers and Communications)</em>, July  2002.

        <a target="_blank" href="http://www.cs.ucla.edu/~lixia/papers/02ISCC.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=140" title="Beichuan Zhang, Sugih Jamin, and L. Zhang, &lt;strong&gt;&amp;quot;Host Multicast: A Framework for Delivering Multicast to End Users&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE INFOCOM&lt;/em&gt;, June  2002. "><img src="/images/extensions/bib.png" /></a>

     Beichuan Zhang, Sugih Jamin, and L. Zhang, <br/><strong>&quot;Host Multicast: A Framework for Delivering Multicast to End Users</strong>,&quot; <br/><em>IEEE INFOCOM</em>, June  2002.

        <a target="_blank" href="/papers/hmcast_infocom02.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=141" title="D. Pei, X. Zhao, L. Wang, D. Massey, A. Mankin, S. F. Wu, , and L. Zhang, &lt;strong&gt;&amp;quot;Improving BGP Convergence Through Consistency Assertions&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE INFOCOM&lt;/em&gt;, June  2002. "><img src="/images/extensions/bib.png" /></a>

     D. Pei, X. Zhao, L. Wang, D. Massey, A. Mankin, S. F. Wu, , and L. Zhang, <br/><strong>&quot;Improving BGP Convergence Through Consistency Assertions</strong>,&quot; <br/><em>IEEE INFOCOM</em>, June  2002.

        <a target="_blank" href="/papers/dan_infocom2002.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=142" title="Jun Li, Jelena Mirkovic, Mengqiu Wang, Peter Reiher, and Lixia Zhang, &lt;strong&gt;&amp;quot;SAVE: Source Address Validity Enforcement Protocol&lt;/strong&gt;,&amp;quot; &lt;em&gt;INFOCOM&lt;/em&gt;, June  2002. "><img src="/images/extensions/bib.png" /></a>

     Jun Li, Jelena Mirkovic, Mengqiu Wang, Peter Reiher, and Lixia Zhang, <br/><strong>&quot;SAVE: Source Address Validity Enforcement Protocol</strong>,&quot; <br/><em>INFOCOM</em>, June  2002.

        <a target="_blank" href="/papers/save_infocom.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=143" title="Xiaoliang Zhao, Dan Pei, Lan Wang, Dan Massey, Allison Mankin, Felix S. Wu, and Lixia Zhang, &lt;strong&gt;&amp;quot;Detection of Invalid Routing Announcement in the Internet&lt;/strong&gt;,&amp;quot; &lt;em&gt;Proceedings of International Conference on Dependable Systems &amp;amp; Networks (DSN)&lt;/em&gt;, June  2002. "><img src="/images/extensions/bib.png" /></a>

     Xiaoliang Zhao, Dan Pei, Lan Wang, Dan Massey, Allison Mankin, Felix S. Wu, and Lixia Zhang, <br/><strong>&quot;Detection of Invalid Routing Announcement in the Internet</strong>,&quot; <br/><em>Proceedings of International Conference on Dependable Systems &amp; Networks (DSN)</em>, June  2002.

        <a target="_blank" href="/papers/fniisc_dsn02.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=144" title="Jelena Mirkovic, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Self-Organizing Approach to Data Forwarding in Wireless Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;ICC&lt;/em&gt;, June  2002. "><img src="/images/extensions/bib.png" /></a>

     Jelena Mirkovic, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;A Self-Organizing Approach to Data Forwarding in Wireless Sensor Networks</strong>,&quot; <br/><em>ICC</em>, June  2002.

        <a target="_blank" href="/papers/icc2001-jelena.ps"><img src="/images/extensions/ps.png"></a>

    </li>

</ul><h3>2001</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=145" title="J. Kong, P. Zerfos, H. Luo, S. Lu, and L. Zhang, &lt;strong&gt;&amp;quot;Providing robust and ubiquitous security support for MANET&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE International Conference on Network Protocols (ICNP)&lt;/em&gt;, November  2001. "><img src="/images/extensions/bib.png" /></a>

     J. Kong, P. Zerfos, H. Luo, S. Lu, and L. Zhang, <br/><strong>&quot;Providing robust and ubiquitous security support for MANET</strong>,&quot; <br/>in <em>Proceedings of IEEE International Conference on Network Protocols (ICNP)</em>, November  2001.

        <a target="_blank" href="/papers/ICNP01-haiyun.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=146" title="Joe Albowicz, Alvin Chen, and Lixia Zhang, &lt;strong&gt;&amp;quot;Recursive Position Estimation in Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE Internation Conference on Network Protocols (ICNP)&lt;/em&gt;, November  2001. "><img src="/images/extensions/bib.png" /></a>

     Joe Albowicz, Alvin Chen, and Lixia Zhang, <br/><strong>&quot;Recursive Position Estimation in Sensor Networks</strong>,&quot; <br/><em>IEEE Internation Conference on Network Protocols (ICNP)</em>, November  2001.

        <a target="_blank" href="/papers/grab-icnp01.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=147" title="Allison Mankin, Dan Massey, Chie Lung Wu, Felix S. Wu, and Lixia Zhang, &lt;strong&gt;&amp;quot;On Design and Evaluation of &#039;Intention-Driven&#039; ICMP Traceback&lt;/strong&gt;,&amp;quot; &lt;em&gt;10th International Conference on Computer Communications and Networks (IC3N)&lt;/em&gt;, October  2001. "><img src="/images/extensions/bib.png" /></a>

     Allison Mankin, Dan Massey, Chie Lung Wu, Felix S. Wu, and Lixia Zhang, <br/><strong>&quot;On Design and Evaluation of 'Intention-Driven' ICMP Traceback</strong>,&quot; <br/><em>10th International Conference on Computer Communications and Networks (IC3N)</em>, October  2001.

        <a target="_blank" href="/papers/Intention-iTrace.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=148" title="Fan Ye, Alvin Chen, Songwu Lu, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Scalable Solution to Minimum Cost Forwarding in Large Scale Sensor Networks&lt;/strong&gt;,&amp;quot; &lt;em&gt;International Conference on Computer Communications and Networks (IC3N)&lt;/em&gt;, October  2001. "><img src="/images/extensions/bib.png" /></a>

     Fan Ye, Alvin Chen, Songwu Lu, and Lixia Zhang, <br/><strong>&quot;A Scalable Solution to Minimum Cost Forwarding in Large Scale Sensor Networks</strong>,&quot; <br/><em>International Conference on Computer Communications and Networks (IC3N)</em>, October  2001.

        <a target="_blank" href="/papers/grab-icccn01.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=149" title="P. Francis, S. Jamin, C. Jin, Y. Jin, D. Raz, Y. Shavitt, , and L. Zhang, &lt;strong&gt;&amp;quot;IDMAPS: A Global Internet Host Distance Estimate Service&lt;/strong&gt;,&amp;quot; &lt;em&gt;IEEE/ACM Transactions on Networking, Vol. 9, No 5, PP525-540&lt;/em&gt;, October  2001. "><img src="/images/extensions/bib.png" /></a>

     P. Francis, S. Jamin, C. Jin, Y. Jin, D. Raz, Y. Shavitt, , and L. Zhang, <br/><strong>&quot;IDMAPS: A Global Internet Host Distance Estimate Service</strong>,&quot;quot; <br/><em>IEEE/ACM Transactions on Networking, Vol. 9, No 5, PP525-540</em>, October  2001.

        <a target="_blank" href="/papers/ton01-idmaps.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=150" title="Xiaoliang Zhao, Dan Pei, Lan Wang, Dan Massey, Allison Mankin, Felix S. Wu, and Lixia Zhang, &lt;strong&gt;&amp;quot;An Analysis of BGP Multiple Origin AS(MOAS) Conflicts&lt;/strong&gt;,&amp;quot; &lt;em&gt;SIGCOMM Internet Measurement Workshop&lt;/em&gt;, August  2001. "><img src="/images/extensions/bib.png" /></a>

     Xiaoliang Zhao, Dan Pei, Lan Wang, Dan Massey, Allison Mankin, Felix S. Wu, and Lixia Zhang, <br/><strong>&quot;An Analysis of BGP Multiple Origin AS(MOAS) Conflicts</strong>,&quot; <br/><em>SIGCOMM Internet Measurement Workshop</em>, August  2001.

        <a target="_blank" href="/papers/fniisc-sigcomm-workshop01.ps"><img src="/images/extensions/ps.png"></a>

    </li>

</ul><h3>2000</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=151" title="Andreas Terzis, Konstantinos Nikoloudakis, Lan Wang, and Lixia Zhang, &lt;strong&gt;&amp;quot;IRLSim: A general purpose packet level network simulator&lt;/strong&gt;,&amp;quot; &lt;em&gt;33rd Annual Simulation Symposium, Washington D.C.&lt;/em&gt; April  2000. "><img src="/images/extensions/bib.png" /></a>

     Andreas Terzis, Konstantinos Nikoloudakis, Lan Wang, and Lixia Zhang, <br/><strong>&quot;IRLSim: A general purpose packet level network simulator</strong>,&quot; <br/><em>33rd Annual Simulation Symposium, Washington D.C.</em> April  2000.

        <a target="_blank" href="/papers/irlsim.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=152" title="Michel, B. S., Nikoloudakis, K., Reiher, P., , Zhang, and L. &lt;strong&gt;&amp;quot;URL Forwarding and Compression in Adaptive Web Caching&lt;/strong&gt;,&amp;quot; &lt;em&gt;INFOCOM&lt;/em&gt;, March  2000. "><img src="/images/extensions/bib.png" /></a>

     Michel, B. S., Nikoloudakis, K., Reiher, P., , Zhang, and L. <br/><strong>&quot;URL Forwarding and Compression in Adaptive Web Caching</strong>,&quot; <br/><em>INFOCOM</em>, March  2000.

        <a target="_blank" href="http://flapps.cs.ucla.edu/papers/AWC-INFOCOM2K.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=153" title="S. Jamin, C. Jin, Y. Jin, D. Raz, Y. Shavitt, and L. Zhang, &lt;strong&gt;&amp;quot;On the Placement of Internet Instrumentation&lt;/strong&gt;,&amp;quot; &lt;em&gt;INFOCOM&lt;/em&gt;, March  2000. "><img src="/images/extensions/bib.png" /></a>

     S. Jamin, C. Jin, Y. Jin, D. Raz, Y. Shavitt, and L. Zhang, <br/><strong>&quot;On the Placement of Internet Instrumentation</strong>,&quot; <br/><em>INFOCOM</em>, March  2000.

        <a target="_blank" href="http://idmaps.eecs.umich.edu/papers/infocom00.ps"><img src="/images/extensions/ps.png"></a>

    </li>

</ul><h3>1999</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=154" title="Andreas Terzis, Lan Wang, Jun Ogawa, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Two-Tier Resource Management Model for the Internet&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of Global Internet 99&lt;/em&gt;, December  1999. "><img src="/images/extensions/bib.png" /></a>

     Andreas Terzis, Lan Wang, Jun Ogawa, and Lixia Zhang, <br/><strong>&quot;A Two-Tier Resource Management Model for the Internet</strong>,&quot; <br/>in <em>Proceedings of Global Internet 99</em>, December  1999.

        <a target="_blank" href="/papers/paper-final-gi99.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=155" title="C. G. Liu, D. Estrin, S. Shenker, and L. Zhang, &lt;strong&gt;&amp;quot;Recovery Timer Adaptation in SRM&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of ICCC&lt;/em&gt;, October  1999. "><img src="/images/extensions/bib.png" /></a>

     C. G. Liu, D. Estrin, S. Shenker, and L. Zhang, <br/><strong>&quot;Recovery Timer Adaptation in SRM</strong>,&quot; <br/>in <em>Proceedings of ICCC</em>, October  1999.

        <a target="_blank" href="/papers/ICCC99.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=156" title="Lan Wang, Andreas Terzis, and Lixia Zhang, &lt;strong&gt;&amp;quot;A New Proposal for RSVP Refreshes&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 7th International Conference on Network Protocols (ICNP)&lt;/em&gt;, October  1999. "><img src="/images/extensions/bib.png" /></a>

     Lan Wang, Andreas Terzis, and Lixia Zhang, <br/><strong>&quot;A New Proposal for RSVP Refreshes</strong>,&quot; <br/>in <em>Proceedings of the 7th International Conference on Network Protocols (ICNP)</em>, October  1999.

        <a target="_blank" href="/papers/ICNP99.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=157" title="N. Sturtevant, N. Tang, and L. Zhang, &lt;strong&gt;&amp;quot;The Information Discovery Graph: Towards a Scalable Multimedia Resource Directory&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE Workshop on Internet Applications&lt;/em&gt;, July  1999. "><img src="/images/extensions/bib.png" /></a>

     N. Sturtevant, N. Tang, and L. Zhang, <br/><strong>&quot;The Information Discovery Graph: Towards a Scalable Multimedia Resource Directory</strong>,&quot; <br/>in <em>Proceedings of IEEE Workshop on Internet Applications</em>, July  1999.

        <a target="_blank" href="/papers/IDG_WIAPP_paper.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=158" title="Mario Gerla, Rajive Bagrodia, Lixia Zhang, Ken Tang, and Lan Wang, &lt;strong&gt;&amp;quot;TCP over Wireless Multihop Protocols: Simulation and Experiments&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of International Conference on Communications (ICC)&lt;/em&gt;, June  1999. "><img src="/images/extensions/bib.png" /></a>

     Mario Gerla, Rajive Bagrodia, Lixia Zhang, Ken Tang, and Lan Wang, <br/><strong>&quot;TCP over Wireless Multihop Protocols: Simulation and Experiments</strong>,&quot; <br/>in <em>Proceedings of International Conference on Communications (ICC)</em>, June  1999.

        <a target="_blank" href="/papers/icc99.ps"><img src="/images/extensions/ps.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=159" title="Andreas Terzis, Jun Ogawa, Sonia Tsui, Lan Wang, and Lixia Zhang, &lt;strong&gt;&amp;quot;A Prototype Implementation of the Two-Tier Architecture for Differentiated Services&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of RTAS99&lt;/em&gt;, June  1999. "><img src="/images/extensions/bib.png" /></a>

     Andreas Terzis, Jun Ogawa, Sonia Tsui, Lan Wang, and Lixia Zhang, <br/><strong>&quot;A Prototype Implementation of the Two-Tier Architecture for Differentiated Services</strong>,&quot; <br/>in <em>Proceedings of RTAS99</em>, June  1999.

        <a target="_blank" href="/papers/rtas99-final.pdf"><img src="/images/extensions/pdf.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=160" title="A. Terzis, M. Srivastava, and L. Zhang, &lt;strong&gt;&amp;quot;A Simple QoS Signaling Protocol for Mobile Hosts in the Integrated Services Internet&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE INFOCOM&lt;/em&gt;, March  1999. "><img src="/images/extensions/bib.png" /></a>

     A. Terzis, M. Srivastava, and L. Zhang, <br/><strong>&quot;A Simple QoS Signaling Protocol for Mobile Hosts in the Integrated Services Internet</strong>,&quot; <br/>in <em>Proceedings of IEEE INFOCOM</em>, March  1999.

        <a target="_blank" href="/papers/infocom99.ps.gz"><img src="/images/extensions/gz.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=161" title="P. Francis, S. Jamin, V. Paxson, L. Zhang, D. Gryniewicz, and Y. Jin, &lt;strong&gt;&amp;quot;An Architecture for a Global Internet Host Distance Estimation Service&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IEEE INFOCOM&lt;/em&gt;, March  1999. "><img src="/images/extensions/bib.png" /></a>

     P. Francis, S. Jamin, V. Paxson, L. Zhang, D. Gryniewicz, and Y. Jin, <br/><strong>&quot;An Architecture for a Global Internet Host Distance Estimation Service</strong>,&quot; <br/>in <em>Proceedings of IEEE INFOCOM</em>, March  1999.

        <a target="_blank" href="http://idmaps.eecs.umich.edu/papers/infocom99.ps.gz"><img src="/images/extensions/gz.png"></a>

    </li>

</ul><h3>1998</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=162" title="C. Liu, D. Estrin, S. Shenker, and L. Zhang, &lt;strong&gt;&amp;quot;Local Error Recovery in SRM: Comparison of Two Approaches&lt;/strong&gt;,&amp;quot; &lt;em&gt;EEE/ACM Transactions on Networking&lt;/em&gt;, vol. 6, no. 6, pp. 686&amp;ndash;699, December  1998. "><img src="/images/extensions/bib.png" /></a>

     C. Liu, D. Estrin, S. Shenker, and L. Zhang, <br/><strong>&quot;Local Error Recovery in SRM: Comparison of Two Approaches</strong>,&quot; <br/><em>EEE/ACM Transactions on Networking</em>, vol. 6, no. 6, pp. 686&ndash;699, December  1998.

        <a target="_blank" href="/papers/TON_97_1.PS.gz"><img src="/images/extensions/gz.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=163" title="A. Fei, G. Pei, R. Liu, and L. Zhang, &lt;strong&gt;&amp;quot;Measurements on Delay and Hop-Count of the Internet&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of GLOBECOM&lt;/em&gt;, November  1998. "><img src="/images/extensions/bib.png" /></a>

     A. Fei, G. Pei, R. Liu, and L. Zhang, <br/><strong>&quot;Measurements on Delay and Hop-Count of the Internet</strong>,&quot; <br/>in <em>Proceedings of GLOBECOM</em>, November  1998.

        <a target="_blank" href="/papers/internet-measurement.ps.gz"><img src="/images/extensions/gz.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=164" title="A. Terzis, L. Wang, and L. Zhang, &lt;strong&gt;&amp;quot;A Scalable Resource Management Framework for Differentiated Services Internet&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of the 3rd NASA/NREN Workshop on QoS for the Next Generation Internet&lt;/em&gt;, August  1998. "><img src="/images/extensions/bib.png" /></a>

     A. Terzis, L. Wang, and L. Zhang, <br/><strong>&quot;A Scalable Resource Management Framework for Differentiated Services Internet</strong>,&quot; <br/>in <em>Proceedings of the 3rd NASA/NREN Workshop on QoS for the Next Generation Internet</em>, August  1998.

        <a target="_blank" href="/papers/NREN-final.txt"><img src="/images/extensions/txt.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=165" title="A. Terzis, L. Zhang, and E. Hahne, &lt;strong&gt;&amp;quot;Making Reservations for Aggregate Flows: Experiences from an RSVP Tunnels Implementation&lt;/strong&gt;,&amp;quot; in &lt;em&gt;Proceedings of IWQoS&lt;/em&gt;, Napa Valley, CA, May  1998. "><img src="/images/extensions/bib.png" /></a>

     A. Terzis, L. Zhang, and E. Hahne, <br/><strong>&quot;Making Reservations for Aggregate Flows: Experiences from an RSVP Tunnels Implementation</strong>,&quot; <br/>in <em>Proceedings of IWQoS</em>, Napa Valley, CA, May  1998.

        <a target="_blank" href="/papers/rsvp-tunnels-camera.ps.gz"><img src="/images/extensions/gz.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=166" title="R. Bruyeron, B. Hemon, and L. Zhang, &lt;strong&gt;&amp;quot;Exprerimentatons with TCP Selective Acknowledgement&lt;/strong&gt;,&amp;quot; &lt;em&gt;CCR&lt;/em&gt;, vol. 28, no. 2, April  1998. "><img src="/images/extensions/bib.png" /></a>

     R. Bruyeron, B. Hemon, and L. Zhang, <br/><strong>&quot;Exprerimentatons with TCP Selective Acknowledgement</strong>,&quot; <br/><em>CCR</em>, vol. 28, no. 2, April  1998.

        <a target="_blank" href="/papers/sack_exp.ps.gz"><img src="/images/extensions/gz.png"></a>

    </li>



<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=167" title="S. Dao, B. Perry, E. Shek, A. Vellaikal, R. Muntz, L. Zhang, M. Potkonjak, , and O. Wolfson, &lt;strong&gt;&amp;quot;Semantic Multicast: Intelligently Sharing Collaborative Sessions&lt;/strong&gt;,&amp;quot; &lt;em&gt;ACM Computing Survey&lt;/em&gt;, January  1998. "><img src="/images/extensions/bib.png" /></a>

     S. Dao, B. Perry, E. Shek, A. Vellaikal, R. Muntz, L. Zhang, M. Potkonjak, , and O. Wolfson, <br/><strong>&quot;Semantic Multicast: Intelligently Sharing Collaborative Sessions</strong>,&quot; <br/><em>ACM Computing Survey</em>, January  1998.

        <a target="_blank" href="http://www.wins.hrl.com/projects/semcast/semcast_whitepaper.ps"><img src="/images/extensions/ps.png"></a>

    </li>

</ul><h3>1997</h3>
<ul>


<li style="margin-top:14px">
    <a class="smoothbox_small" href="/bibwiki/bibtex?id=168" title="A. Rosenstein, J. Li, and S. Y. Tong, &lt;strong&gt;&amp;quot;MASH: The Multicasting Archie Server Hierearchy&lt;/strong&gt;,&amp;quot; &lt;em&gt;CCR&lt;/em&gt;, vol. 27, no. 3, July  1997. "><img src="/images/extensions/bib.png" /></a>

     A. Rosenstein, J. Li, and S. Y. Tong, <br/><strong>&quot;MASH: The Multicasting Archie Server Hierearchy</strong>,&quot; <br/><em>CCR</em>, vol. 27, no. 3, July  1997.

        <a target="_blank" href="http://www.cs.ucla.edu/%7Eadam/report.ps.gz"><img src="/images/extensions/gz.png"></a>

    </li>

    </ul>
</div>