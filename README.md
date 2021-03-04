# start_maven

```
$ java --version
openjdk 11.0.9.1 2020-11-04 LTS
OpenJDK Runtime Environment Corretto-11.0.9.12.1 (build 11.0.9.1+12-LTS)
OpenJDK 64-Bit Server VM Corretto-11.0.9.12.1 (build 11.0.9.1+12-LTS, mixed mode)
```



プロジェクト作成

```
mvn archetype:generate -DgroupId=com.nashiki.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```


"ソース・オプション5は現在サポートされていません。6以降を使用してください"というエラーが出たので、
maven-compiler-plugin を変更した。

https://www.it-swarm.jp.net/ja/eclipse/maven%E3%82%B3%E3%83%B3%E3%83%91%E3%82%A4%E3%83%AB%E6%99%82%E3%81%AE%E3%82%A8%E3%83%A9%E3%83%BC%E3%80%8C%E3%82%BD%E3%83%BC%E3%82%B9%E3%82%AA%E3%83%97%E3%82%B7%E3%83%A7%E3%83%B35%E3%81%AF%E3%82%B5%E3%83%9D%E3%83%BC%E3%83%88%E3%81%95%E3%82%8C%E3%81%A6%E3%81%84%E3%81%BE%E3%81%9B%E3%82%93%E3%80%826%E4%BB%A5%E9%99%8D%E3%82%92%E4%BD%BF%E7%94%A8%E3%81%97%E3%81%A6%E3%81%8F%E3%81%A0%E3%81%95%E3%81%84%E3%80%8D/806748901/

```
~/ghq/github.com/nnashiki/start_maven/my-app
$ mvn compile

$ java -cp target/classes com.nashiki.app.App       
Hello World!

$ mvn compile exec:java
```

```
$ mvn compiler:testCompile
$ mvn test
```



参考記事

- https://speakerdeck.com/yusuke/madajian-nihe-umaven-zai-ru-men-number-jjug?slide=27
