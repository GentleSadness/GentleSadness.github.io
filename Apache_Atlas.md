### Building & Installing Apache Atlas

`tar -xzvf apache-atlas-${project.version}-server.tar.gz`，使用server包，而不是bin包

### Apache Atlas Hook & Bridge for Apache HBase

```
<property>
<name>hbase.coprocessor.master.classes</name>
<value>org.apache.atlas.hbase.hook.HBaseAtlasCoprocessor</value>
</property>
```

可知，Hook入口类为HBaseAtlasCoprocessor。
