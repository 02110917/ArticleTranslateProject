---
layout: post
title: Architecting Android��The clean way?
categories: [Android]
tags: [Android,MVP]
description:
fullview: true
---
<html>
<head>
<meta charset="utf-8">
<title>2014-09-11-Architecting Android��The clean way.md</title>
<link rel="stylesheet" href="https://stackedit.io/res-min/themes/base.css" />
<script type="text/javascript" src="https://stackedit.io/libs/MathJax/MathJax.js?config=TeX-AMS_HTML"></script>
</head>
<body><div class="container"><hr>

<blockquote>
  <p><strong><em>Edit by Fooyou Email : <a href="mailto:foyou23@qq.com">foyou23@qq.com</a> 2000-10-10 </em></strong> </p>
</blockquote>



<hr>



<h2 id="architecting-androidthe-clean-way"><strong>Architecting Android��The clean way?</strong></h2>

<p><a href="http://fernandocejas.com/2014/09/03/architecting-android-the-clean-way/">����ԭ��</a></p>

<p>�ڹ�ȥ�ļ����£�Ҳ���ǣ���<a href="http://corporate.tuenti.com/en/dev/blog"> Tuenti </a> ��ʱ�򣬸���2��ͬ�� <a href="https://twitter.com/pedro_g_s">@pedro_g_s</a> �� <a href="https://twitter.com/flipper83"> @flipper83</a> <em>��˳�����£�����2������Android�����Ļ��һ</em>��������һ���Ѻõ�����֮���Ҿ;�������ʱ��дһƪ������<strong>Android Ӧ�ÿ��</strong>�������ˡ�</p>

<p>��ƪ���µ�Ŀ�ģ��������չʾһ�����⼸��������ģ��Լ�����������ʵ�֣������ܣ������� ��ѧ����������ص����ݡ�</p>



<h3 id="��ʼ��getting-started">��ʼ�ɣ�Getting Started��</h3>

<p><strong>���Ƕ�֪����Ҫдһ�����ʵ������ͦ���Ѻ͸��ӵ�</strong>������Ҫ����������󣬻�Ҫ������������׳�ȶ�����ά���ԣ��ײ����ԣ�����Ҫ�㹻��������������ºͱ仯�������Ϊʲô Ҫ�ᳫ<strong>��һ�����ļܹ���the clean architecture����</strong>���������ڿ����κ����Ӧ�õ�ʱ���ܹ��ܷ����ʹ������</p>

<p>���˼·�ܼ򵥣�<strong>���ܹ�</strong> ��ζ�Ų�Ʒϵͳ����ѭһϵ�е�ϰ��ԭ��</p>

<ul>
<li><strong>��ܶ�����</strong></li>
<li><strong>�ɲ���</strong></li>
<li><strong>UI������</strong></li>
<li><strong>���ݿ������</strong></li>
<li><strong>�κ��ⲿ����ģ��Ķ�����</strong></li>
</ul>

<p><img src="http://fernandocejas.com/wp-content/uploads/2014/09/clean_architecture1.png" alt="enter image description here" title=""></p>

<p>Ҳ����һ��ֻ��4ԲȦ������ͼ��ʾ������Ϊ��ֻ�Ǹ�ʾ�������ǣ�������뿼�� <strong>����ԭ��Dependency Rule��</strong>��Դ������ֻ�����������ڵģ����У�<strong>�ڻ�</strong>������κζ���������Ҫ֪��<strong>�⻷</strong>�κ�ʵ�ַ�ʽ��<em>�� ���ߣ���˵���ǣ�<code>�⻷</code>��������<code>�ڻ�</code>����������<code>�ڻ�</code>�Ķ���������<code>�⻷</code>�ģ�����<code>�⻷</code>���ݸı���ܵ�Ӱ�죬���ң�<code>�ڻ�</code>Ҳ����Ҫ֪��<code>�⻷</code>����κξ����߼�ʵ�֡���</em></p>

<blockquote>
  <p><em>���ߣ������ܲ���������������̫��Ť�ˣ�Ϊ�˾����ܵı���ԭ��ԭζ�ķ��룬��Ը������Լ���������֯�����ǣ�����������˼�ֲ����������ӵ�������Ūѽ��</em></p>
</blockquote>

<p>�����ǽ���һЩ�ʻ����Ϊ���������Ϥ�������������ƪ���¡�</p>

<ul>
<li><strong>Entities��</strong> ��Щ��ָӦ�õ� <code>ҵ�����</code>��<em>�����ߣ�����ģ���࣬ʵ���࣬��Java����</em></li>
<li><strong>Use Cases��</strong> ��Щ��ָ<code>����</code>�������ݺ�ҵ�����������������Ҳ���Խ���Լ������<em>�����ߣ���˵�������ݹ�����������������Լ�����ȵȡ���</em></li>
<li><strong>Interface Adapters��</strong> ��һ�����������Ǹ����������ĸ�ʽת��<code>����</code>��<code>use cases</code>����<code>ʵ��</code>��<code>entities</code>��֮������ݣ�<strong>���ֲ�</strong>��Presenters ����<strong>���Ʋ�</strong>��Controllers ������������һ��ġ�</li>
<li><strong>Frameworks and Drivers:</strong> ���������о����ʵ���ˣ����磺UI�������࣬������ܣ��ȵȡ�</li>
</ul>

<p>��Ҫ�����壬�������ḻ�Ľ��ͣ����Բο�<a href="http://blog.8thlight.com/uncle-bob/2012/08/13/the-clean-architecture.html">��ƪ����</a>����<a href="http://vimeo.com/43612849">�����Ƶ</a></p>

<blockquote>
  <p>������Ƶ������Ҫ��ǽ������Ұﲻ����� ��XD</p>
</blockquote>



<h3 id="���ǵİ���-our-scenario">���ǵİ����� Our Scenario��</h3>

<p>�һ���һ���򵥵İ�������ʵ��һ�£��򵥴���һ��Ӧ�ã����Ӧ����������ʾһ�������б�������ʾ�ƶ˵��û������ظ�����������Щ�κ�һ����Ŀ��ʱ�򣬻��һ���µĽ��棬չʾ����û�����ϸ�����ݡ� <br>
�Ҹ�����һ����Ƶ���������ܸ�ֱ�۵Ŀ����������������ݣ�</p>

<iframe width="640" height="480" src="//www.youtube.com/embed/XSjV4sG3ni0" allowfullscreen=""></iframe>

<blockquote>
  <p>�����һ��Ҫ��ǽ����Ƶ��Youtube��ַ���Ұﲻ��������</p>
</blockquote>



<h3 id="android�ܹ�-android-architecture">Android�ܹ� ��Android Architecture��</h3>

<p>����ҪĿ����<strong>�������루separation of concerns �����</strong> ����֤ҵ���߼����漰�κ��⻷��������ݣ����������ǾͿ��Ժܷ���Ĳ��ԣ�����Ҫ�����κ��ⲿԪ�ء�</p>

<p>Ҫ������һ���أ��ҵĽ����ǰ�������Ŀ��ֳ�3����ͬ�Ĳ㼶��ÿһ�㶼�Ǹ��Թ��ܣ���������֮�䱣�ֶ����� <br>
ֵ��һ����ǣ�ÿһ�㶼ʹ�������Լ�������ģ�ͣ��������������������������㽫�ᷢ���ڴ������棬��Ҫ��һ������ӳ�䣬���ܸ��õ��������ת�����䣬��ô�����ǻḶ��һЩ���۵ģ�������ģ�͵�ʹ�ò��ǹᴩ����Ӧ�õĻ�����</p>

<blockquote>
  <p>��ͼ��һ������ṹ�������ֱ�۵Ŀ������������ô���ġ�</p>
</blockquote>

<p><img src="http://fernandocejas.com/wp-content/uploads/2014/09/clean_architecture_android.png" alt="enter image description here" title=""></p>

<p><strong>˵����</strong> ��û��ʹ���κ��������ⲿ�⣨����ʹ����<code>gson</code> ��json���ݽ���������ʹ�ã�<code>junit</code>��<code>mockito</code>��robolectric ��<code>espresso</code> �������ԣ���ԭ������Ϊ����������ʹ��Ŀ���Ӽ򵥣�������ô������Ҫ��ԥʹ�ã�ORMs�������ϵӳ�䣩�����ݴ洢�����������κ�����ע��Ŀ�ܣ���������һЩ�������ƵĿ�ܣ�����������ʹ�����ĸ�������<strong>����ס���ظ������Ӳ���һ����ϰ��Ŷ��</strong></p>



<h3 id="���ֲ�presentation-layer">���ֲ㣨Presentation Layer��</h3>

<p>�����������һЩ����ͼ�Ͷ�����ص��߼��ˣ�ʹ��<strong>Model View Presenter</strong> ģʽ����ò������ˣ�������<a href="http://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93presenter">MVP</a>������Ȼ�ˣ������ʹ���������Ƶģ����� <code>MVC</code> ���� <code>MVVM</code> �����Ҳ���������ˣ������������ֻ��<strong>fragments</strong> ��<strong>activities</strong> ������<code>��ͼ</code>���������д�ģ�����UI��ص��߼�֮�⣬û�б���ˣ����⣬��Ⱦ�滭��ص�����Ҳ���������������<strong>Presenters</strong>  ������� interactors (use cases)�������̣߳���UI�߳�֮�⴦������߼���Ȼ��ͨ���ص��ķ�ʽ�����ݷ��ص���ͼģ�顣</p>

<p><img src="http://fernandocejas.com/wp-content/uploads/2014/09/clean_architecture_mvp.png" alt="enter image description here" title=""></p>

<p>�������Ҫһ����������ӣ����Կ���<a href="https://github.com/pedrovgs/EffectiveAndroidUI/">Effective Android UI</a>��Ҳ��ʹ���� <code>MVP</code> �� <code>MVVM</code>������������ Pedro G��mez д����ô����</p>



<h3 id="�����-domain-layer">����� ��Domain Layer��</h3>

<p><strong><code>ҵ���߼�</code>�����⣺����ҵ����ص����ݶ�������һ�㡣</strong>��Android ��Ŀ��˵�Ļ�����ᷢ�����е�����interactors (use cases)ʵ��Ҳ��������һ�㡣 <br>
��һ���Ǵ� <code>Java</code> ��д�ģ�û���κ�Android��ص������������ⲿ�������ͨ���ӿڵķ�ʽ����ҵ���߼���</p>

<p><img src="http://fernandocejas.com/wp-content/uploads/2014/09/clean_architecture_domain.png" alt="enter image description here" title=""></p>



<h3 id="���ݲ�data-layer">���ݲ㣨Data Layer��</h3>

<p>����Ӧ�����ݵĻ�ȡ������������һ�㣬��<code>�û��ֿ�</code>��UserRepository ����ʵ�ַ�ʽ���ӿ��Ƕ�����<code>�����</code>�ģ���ʹ�� �ֿ�ģʽ��<a href="http://martinfowler.com/eaaCatalog/repository.html">Repository Pattern</a>�������Ĳ����ǲ��ù���ģʽ�����ݲ�ͬ��������������ȡ��ͬ�����ݡ� <br>
���磺ͨ��ID�����û�������û�������������Ļ����ͻ�����ʹ�ô��̻������ݣ����û�У��ͻ������������ݣ���ɺ󣬱��浽���̡� <br>
�ⱳ���˼·���ǣ�ԭʼ�����ǶԿͻ���͸���ģ��ͻ��˲���Ҫ��ע���������������ڴ棬���Ǵ��̣����߷������ƶˣ�ֻҪ�����ݴ��ݳ�ȥ��Ҳ��ȡ�����͹��ˡ�</p>

<p><img src="http://fernandocejas.com/wp-content/uploads/2014/09/clean_architecture_data.png" alt="enter image description here" title=""></p>

<p><strong>˵����</strong>����δ����У���ʵ�ֵıȽϼ򵥣�ʹ����ԭ�����ļ�ϵͳ�洢��<code>Android</code> preferences�����ļ���ʽ�������̻��棬ֻ��Ϊ�˴ﵽѧϰĿ�ģ����ǵ�����һ�£�<strong>��Ҫ�ظ�������</strong>����������еĳ���Ŀ�������Щ�����Ļ���</p>



<h3 id="������-error-handling">������ ��Error Handling��</h3>

<p>����һ���������۵Ļ����ˣ�������кܺõķ�����Ҫ����Ļ����ǻ���á�<strong>�ҵĽ�����ʹ�� �ص�</strong>�����������磺��������ݲֿⷢ������Ļ�������ͨ�����ã��ص��ӿڵ�2��������<strong>onResponse()</strong> �� <strong>onError()</strong>������һ������������һ����װ�˸����쳣���ݵ��� <strong>��ErrorBundle��</strong>�������������һЩ�鷳����Ϊ��һ�����Ļص��ӿڣ�һ����һ�����ڴ��󴫵ݵ����ֲ㣬����ɶ��Իή�ͣ���һ���� <br>
�һ�ʵ����һ���¼�����ϵͳ������д��������ͻ��׳��¼����ͺ���ʹ��<a href="http://www.drdobbs.com/jvm/programming-with-reason-why-is-goto-bad/228200966">GOTO</a>һ�������ң����ҿ�������ʱ�������ҵģ���������˺ܶ���¼�������û�к���Ŀ��ƵĻ���</p>



<h3 id="����-testing">���� ��Testing��</h3>

<p>���ڲ��ԣ��Ҳ����˺ü������������ȡ������ĸ����ֲ㣺</p>

<ul>
<li><strong>Presentation Layer��</strong> ʹ��Android�Դ���<code>instrumentation</code> ��<code>espresso</code>  �����ɺ͹��ܲ��ԡ�</li>
<li><strong>Domain Layer:</strong> <code>JUnit</code> + <code>mockito</code>����Ԫ���ԡ�</li>
<li><strong>Data Layer:</strong> <code>Robolectric</code> ����һ�㿪ʼ��Android��ص�������+<code>junit</code> +<code>mockito</code>  ����Ԫ�ͼ��ɲ��ԡ�</li>
</ul>

<h3 id="����չʾshow-me-the-code">����չʾ��Show me the code��</h3>

<p><strong>��֪�������֪�����������أ��Բ��ԣ� </strong> �ðѣ�<a href="https://github.com/android10/Android-CleanArchitecture">������github���ӵ�ַ</a> ������������ҵ���д�ģ�����Ŀ¼�ṹ��һЩҪ˵���ģ����ǣ���ͬ�Ĳ㣬ʹ�ò�ͬ��ģ�飺</p>

<ul>
<li><strong>presentation:</strong> Androidģ�飬����presentation ���ֲ�����ݡ�</li>
<li><strong> domain��</strong> Javaģ�飬������Android��صĶ�����</li>
<li><strong>data:</strong> Androidģ�飬������Դ�ĵط����� ���ݶ��Ǵ����ȡ��</li>
<li><strong>data-test:</strong>  ���ݲ���ԣ���Ϊ<code>Robolectric</code> ��һЩ���ƣ��Ұ����ֳɼ���javaģ�顣</li>
</ul>



<h3 id="�ܽ�conclusion">�ܽᣨConclusion��</h3>

<p>���� <code>Uncle Bob</code> ��˵��<strong>��Architecture is About Intent, not Frameworks��</strong> ���ҷǳ�ͬ�����˵������Ȼ�ˣ��кܶ಻ͬ�ķ�������ͬ�����飨��ͬ��ʵ�ַ��������Һ�ȷ������ÿ�죨����һ���������ٺܶ���ս��������ѭ��Щ������ȷ����Ӧ���������¼��㣺</p>

<ul>
<li><strong>��ά�� Easy to maintain</strong></li>
<li><strong>�ײ��� Easy to test.</strong></li>
<li><strong>�߾ۺ�Very cohesive.</strong></li>
<li><strong>����� Decoupled.</strong> <br>
�����ǿ���Ƽ���ȥ����һ�£�ʵ�������ҷ�����ľ��顣Ҳ������ҵ����õĽ�����������Ƕ�֪����<strong>��������</strong>һ�����ǳ��õģ��ǳ�����������ѽ����ϣ����ƪ���¶���������������ӭ���ַ�����</li>
</ul>



<h3 id="������Դlinks-and-resources">������Դ��Links and Resources��</h3>

<ol>
<li>Source code: <a href="https://github.com/android10/Android-CleanArchitecture">https://github.com/android10/Android-CleanArchitecture</a></li>
<li><a href="http://blog.8thlight.com/uncle-bob/2012/08/13/the-clean-architecture.html">The clean architecture by Uncle Bob</a></li>
<li><a href="http://www.infoq.com/news/2013/07/architecture_intent_frameworks">Architecture is about Intent, not Frameworks</a></li>
<li><a href="http://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93presenter">Model View Presenter</a></li>
<li><a href="http://martinfowler.com/eaaCatalog/repository.html">Repository Pattern by Martin Fowler</a></li>
<li><a href="http://www.slideshare.net/PedroVicenteGmezSnch/">Android Design Patterns Presentation</a></li>
</ol>

<p>Tagged as: android, androiddev, architecture, clean, clean architecture, developer, developers, development, model view presenter, mvp, pattern, patterns, programming, repository, repository pattern, strategy pattern</p></div></body>
</html>