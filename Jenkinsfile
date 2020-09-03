pipeline {
    agent any

    stages {
        stage ('Set Build Tag') {

            steps {
                sh 'ls'
            }
        }

        stage ('Starting some job') {
            
            steps {
                 sh 'ls'
            }
        }
        
        stage ('Jira update') {

            steps {
                sh 'ls -l'
            }
        }
        
        stage ('Release Auto-cherry-pick') {

            steps {
                sh 'ls -l'
            }
        }
        stage ('Parallel') {
            parallel {
                stage ('bazelTest') {
                    steps {
                        sh 'ls -l'
                    }
                }
                stage ('tpch') {
                    steps {
                        sh 'mvn test'
                    }
                }
                stage ('tsPackage') {
                    steps {
                        sh '''echo "Started LevelOps Monitoring Worker Thread
Jul 08, 2020 2:58:14 PM INFO hudson.model.AsyncPeriodicWork lambda$doRun$0
Finished LevelOps Monitoring Worker Thread. 1 ms
Jul 08, 2020 2:58:15 PM WARNING io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$1 onFailure
Exec Failure
java.util.concurrent.RejectedExecutionException: Task okhttp3.RealCall$AsyncCall@2043dd14 rejected from java.util.concurrent.ThreadPoolExecutor@70d6b840[Terminated, pool size = 0, active threads = 0, queued tasks = 0, completed tasks = 27]
	at java.util.concurrent.ThreadPoolExecutor$AbortPolicy.rejectedExecution(ThreadPoolExecutor.java:2063)
	at java.util.concurrent.ThreadPoolExecutor.reject(ThreadPoolExecutor.java:830)
	at java.util.concurrent.ThreadPoolExecutor.execute(ThreadPoolExecutor.java:1379)
	at okhttp3.RealCall$AsyncCall.executeOn(RealCall.java:183)
Caused: java.io.InterruptedIOException: executor rejected
	at okhttp3.RealCall$AsyncCall.executeOn(RealCall.java:186)
	at okhttp3.Dispatcher.promoteAndExecute(Dispatcher.java:186)
	at okhttp3.Dispatcher.enqueue(Dispatcher.java:137)
	at okhttp3.RealCall.enqueue(RealCall.java:127)
	at okhttp3.internal.ws.RealWebSocket.connect(RealWebSocket.java:193)
	at okhttp3.OkHttpClient.newWebSocket(OkHttpClient.java:435)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager.runWatch(WatchConnectionManager.java:161)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager.access$1500(WatchConnectionManager.java:50)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$2$1.execute(WatchConnectionManager.java:334)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$NamedRunnable.run(WatchConnectionManager.java:423)
	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:511)
	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.access$201(ScheduledThreadPoolExecutor.java:180)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.run(ScheduledThreadPoolExecutor.java:293)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624)
	at java.lang.Thread.run(Thread.java:748)

Jul 08, 2020 2:58:27 PM INFO hudson.model.AsyncPeriodicWork lambda$doRun$0
Started jobAnalytics
Jul 08, 2020 2:58:27 PM INFO hudson.model.AsyncPeriodicWork lambda$doRun$0
Finished jobAnalytics. 1 ms
Jul 08, 2020 2:58:47 PM WARNING io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$1 onFailure
Exec Failure
java.util.concurrent.RejectedExecutionException: Task okhttp3.RealCall$AsyncCall@dd2c14b rejected from java.util.concurrent.ThreadPoolExecutor@70d6b840[Terminated, pool size = 0, active threads = 0, queued tasks = 0, completed tasks = 27]
	at java.util.concurrent.ThreadPoolExecutor$AbortPolicy.rejectedExecution(ThreadPoolExecutor.java:2063)
	at java.util.concurrent.ThreadPoolExecutor.reject(ThreadPoolExecutor.java:830)
	at java.util.concurrent.ThreadPoolExecutor.execute(ThreadPoolExecutor.java:1379)
	at okhttp3.RealCall$AsyncCall.executeOn(RealCall.java:183)
Caused: java.io.InterruptedIOException: executor rejected
	at okhttp3.RealCall$AsyncCall.executeOn(RealCall.java:186)
	at okhttp3.Dispatcher.promoteAndExecute(Dispatcher.java:186)
	at okhttp3.Dispatcher.enqueue(Dispatcher.java:137)
	at okhttp3.RealCall.enqueue(RealCall.java:127)
	at okhttp3.internal.ws.RealWebSocket.connect(RealWebSocket.java:193)
	at okhttp3.OkHttpClient.newWebSocket(OkHttpClient.java:435)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager.runWatch(WatchConnectionManager.java:161)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager.access$1500(WatchConnectionManager.java:50)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$2$1.execute(WatchConnectionManager.java:334)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$NamedRunnable.run(WatchConnectionManager.java:423)
	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:511)
	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.access$201(ScheduledThreadPoolExecutor.java:180)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.run(ScheduledThreadPoolExecutor.java:293)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624)
	at java.lang.Thread.run(Thread.java:748)

Jul 08, 2020 2:59:14 PM INFO hudson.model.AsyncPeriodicWork lambda$doRun$0
Started LevelOps Monitoring Worker Thread
Jul 08, 2020 2:59:14 PM INFO hudson.model.AsyncPeriodicWork lambda$doRun$0
Finished LevelOps Monitoring Worker Thread. 1 ms
Jul 08, 2020 2:59:19 PM WARNING io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$1 onFailure
Exec Failure
java.util.concurrent.RejectedExecutionException: Task okhttp3.RealCall$AsyncCall@70d20c59 rejected from java.util.concurrent.ThreadPoolExecutor@70d6b840[Terminated, pool size = 0, active threads = 0, queued tasks = 0, completed tasks = 27]
	at java.util.concurrent.ThreadPoolExecutor$AbortPolicy.rejectedExecution(ThreadPoolExecutor.java:2063)
	at java.util.concurrent.ThreadPoolExecutor.reject(ThreadPoolExecutor.java:830)
	at java.util.concurrent.ThreadPoolExecutor.execute(ThreadPoolExecutor.java:1379)
	at okhttp3.RealCall$AsyncCall.executeOn(RealCall.java:183)
Caused: java.io.InterruptedIOException: executor rejected
	at okhttp3.RealCall$AsyncCall.executeOn(RealCall.java:186)
	at okhttp3.Dispatcher.promoteAndExecute(Dispatcher.java:186)
	at okhttp3.Dispatcher.enqueue(Dispatcher.java:137)
	at okhttp3.RealCall.enqueue(RealCall.java:127)
	at okhttp3.internal.ws.RealWebSocket.connect(RealWebSocket.java:193)
	at okhttp3.OkHttpClient.newWebSocket(OkHttpClient.java:435)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager.runWatch(WatchConnectionManager.java:161)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager.access$1500(WatchConnectionManager.java:50)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$2$1.execute(WatchConnectionManager.java:334)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$NamedRunnable.run(WatchConnectionManager.java:423)
	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:511)
	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.access$201(ScheduledThreadPoolExecutor.java:180)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.run(ScheduledThreadPoolExecutor.java:293)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624)
	at java.lang.Thread.run(Thread.java:748)

Jul 08, 2020 2:59:26 PM INFO org.jenkinsci.plugins.workflow.job.WorkflowRun finish
Operation/pod-reachability-check #3638 completed: SUCCESS
Jul 08, 2020 2:59:40 PM INFO hudson.model.AsyncPeriodicWork lambda$doRun$0
Started LevelOps Monitoring Worker Thread
Jul 08, 2020 2:59:41 PM WARNING io.levelops.plugins.jenkins.extensions.LevelOpsMonitoringPeriodicWork monitorNow
Cannot perform monitoring. Please be sure jenkins/hudson has write privileges in the configured path.
com.fasterxml.jackson.databind.JsonMappingException: Null key for a Map not allowed in JSON (use a converting NullKeySerializer?) (through reference chain: io.levelops.plugins.jenkins.models.PluginResultDTO["results"]->java.util.HashMap["jenkins_config"]->io.levelops.plugins.jenkins.models.jenkins.output.LevelOpsJenkinsData["plugins"]->java.util.HashMap["null"])
	at com.fasterxml.jackson.databind.JsonMappingException.from(JsonMappingException.java:285)
	at com.fasterxml.jackson.databind.SerializerProvider.mappingException(SerializerProvider.java:1251)
	at com.fasterxml.jackson.databind.SerializerProvider.reportMappingProblem(SerializerProvider.java:1145)
	at com.fasterxml.jackson.databind.ser.impl.FailingSerializer.serialize(FailingSerializer.java:35)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serializeFields(MapSerializer.java:705)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serialize(MapSerializer.java:643)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serialize(MapSerializer.java:33)
	at com.fasterxml.jackson.databind.ser.BeanPropertyWriter.serializeAsField(BeanPropertyWriter.java:727)
	at com.fasterxml.jackson.databind.ser.std.BeanSerializerBase.serializeFields(BeanSerializerBase.java:719)
	at com.fasterxml.jackson.databind.ser.BeanSerializer.serialize(BeanSerializer.java:155)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serializeFields(MapSerializer.java:722)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serialize(MapSerializer.java:643)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serialize(MapSerializer.java:33)
	at com.fasterxml.jackson.databind.ser.BeanPropertyWriter.serializeAsField(BeanPropertyWriter.java:727)
	at com.fasterxml.jackson.databind.ser.std.BeanSerializerBase.serializeFields(BeanSerializerBase.java:719)
	at com.fasterxml.jackson.databind.ser.BeanSerializer.serialize(BeanSerializer.java:155)
	at com.fasterxml.jackson.databind.ser.DefaultSerializerProvider._serialize(DefaultSerializerProvider.java:480)
	at com.fasterxml.jackson.databind.ser.DefaultSerializerProvider.serializeValue(DefaultSerializerProvider.java:319)
	at com.fasterxml.jackson.databind.ObjectMapper._configAndWriteValue(ObjectMapper.java:3905)
	at com.fasterxml.jackson.databind.ObjectMapper.writeValueAsString(ObjectMapper.java:3219)
	at io.levelops.plugins.jenkins.service.LevelOpsService2.submitArtifact(LevelOpsService2.java:54)
	at io.levelops.plugins.jenkins.monitoring.HudsonMonitoring.sendDataToLevelOps(HudsonMonitoring.java:144)
	at io.levelops.plugins.jenkins.monitoring.HudsonMonitoring.monitor(HudsonMonitoring.java:124)
	at io.levelops.plugins.jenkins.extensions.LevelOpsMonitoringPeriodicWork.monitorNow(LevelOpsMonitoringPeriodicWork.java:63)
	at io.levelops.plugins.jenkins.extensions.LevelOpsMgmtLink$1.execute(LevelOpsMgmtLink.java:72)
	at hudson.model.AsyncPeriodicWork.lambda$doRun$0(AsyncPeriodicWork.java:100)
	at java.lang.Thread.run(Thread.java:748)

Jul 08, 2020 2:59:41 PM INFO hudson.model.AsyncPeriodicWork lambda$doRun$0
Finished LevelOps Monitoring Worker Thread. 792 ms
Jul 08, 2020 2:59:51 PM WARNING io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$1 onFailure
Exec Failure
java.util.concurrent.RejectedExecutionException: Task okhttp3.RealCall$AsyncCall@24faf44c rejected from java.util.concurrent.ThreadPoolExecutor@70d6b840[Terminated, pool size = 0, active threads = 0, queued tasks = 0, completed tasks = 27]
	at java.util.concurrent.ThreadPoolExecutor$AbortPolicy.rejectedExecution(ThreadPoolExecutor.java:2063)
	at java.util.concurrent.ThreadPoolExecutor.reject(ThreadPoolExecutor.java:830)
	at java.util.concurrent.ThreadPoolExecutor.execute(ThreadPoolExecutor.java:1379)
	at okhttp3.RealCall$AsyncCall.executeOn(RealCall.java:183)
Caused: java.io.InterruptedIOException: executor rejected
	at okhttp3.RealCall$AsyncCall.executeOn(RealCall.java:186)
	at okhttp3.Dispatcher.promoteAndExecute(Dispatcher.java:186)
	at okhttp3.Dispatcher.enqueue(Dispatcher.java:137)
	at okhttp3.RealCall.enqueue(RealCall.java:127)
	at okhttp3.internal.ws.RealWebSocket.connect(RealWebSocket.java:193)
	at okhttp3.OkHttpClient.newWebSocket(OkHttpClient.java:435)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager.runWatch(WatchConnectionManager.java:161)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager.access$1500(WatchConnectionManager.java:50)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$2$1.execute(WatchConnectionManager.java:334)
	at io.fabric8.kubernetes.client.dsl.internal.WatchConnectionManager$NamedRunnable.run(WatchConnectionManager.java:423)
	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:511)
	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.access$201(ScheduledThreadPoolExecutor.java:180)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.run(ScheduledThreadPoolExecutor.java:293)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624)
	at java.lang.Thread.run(Thread.java:748)

Jul 08, 2020 3:00:14 PM INFO hudson.model.AsyncPeriodicWork lambda$doRun$0
Started LevelOps Monitoring Worker Thread
Jul 08, 2020 3:00:15 PM WARNING io.levelops.plugins.jenkins.extensions.LevelOpsMonitoringPeriodicWork monitorNow
Cannot perform monitoring. Please be sure jenkins/hudson has write privileges in the configured path.
com.fasterxml.jackson.databind.JsonMappingException: Null key for a Map not allowed in JSON (use a converting NullKeySerializer?) (through reference chain: io.levelops.plugins.jenkins.models.PluginResultDTO["results"]->java.util.HashMap["jenkins_config"]->io.levelops.plugins.jenkins.models.jenkins.output.LevelOpsJenkinsData["plugins"]->java.util.HashMap["null"])
	at com.fasterxml.jackson.databind.JsonMappingException.from(JsonMappingException.java:285)
	at com.fasterxml.jackson.databind.SerializerProvider.mappingException(SerializerProvider.java:1251)
	at com.fasterxml.jackson.databind.SerializerProvider.reportMappingProblem(SerializerProvider.java:1145)
	at com.fasterxml.jackson.databind.ser.impl.FailingSerializer.serialize(FailingSerializer.java:35)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serializeFields(MapSerializer.java:705)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serialize(MapSerializer.java:643)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serialize(MapSerializer.java:33)
	at com.fasterxml.jackson.databind.ser.BeanPropertyWriter.serializeAsField(BeanPropertyWriter.java:727)
	at com.fasterxml.jackson.databind.ser.std.BeanSerializerBase.serializeFields(BeanSerializerBase.java:719)
	at com.fasterxml.jackson.databind.ser.BeanSerializer.serialize(BeanSerializer.java:155)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serializeFields(MapSerializer.java:722)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serialize(MapSerializer.java:643)
	at com.fasterxml.jackson.databind.ser.std.MapSerializer.serialize(MapSerializer.java:33)
	at com.fasterxml.jackson.databind.ser.BeanPropertyWriter.serializeAsField(BeanPropertyWriter.java:727)
	at com.fasterxml.jackson.databind.ser.std.BeanSerializerBase.serializeFields(BeanSerializerBase.java:719)
	at com.fasterxml.jackson.databind.ser.BeanSerializer.serialize(BeanSerializer.java:155)
	at com.fasterxml.jackson.databind.ser.DefaultSerializerProvider._serialize(DefaultSerializerProvider.java:480)
	at com.fasterxml.jackson.databind.ser.DefaultSerializerProvider.serializeValue(DefaultSerializerProvider.java:319)
	at com.fasterxml.jackson.databind.ObjectMapper._configAndWriteValue(ObjectMapper.java:3905)
	at com.fasterxml.jackson.databind.ObjectMapper.writeValueAsString(ObjectMapper.java:3219)
	at io.levelops.plugins.jenkins.service.LevelOpsService2.submitArtifact(LevelOpsService2.java:54)
	at io.levelops.plugins.jenkins.monitoring.HudsonMonitoring.sendDataToLevelOps(HudsonMonitoring.java:144)
	at io.levelops.plugins.jenkins.monitoring.HudsonMonitoring.monitor(HudsonMonitoring.java:124)
	at io.levelops.plugins.jenkins.extensions.LevelOpsMonitoringPeriodicWork.monitorNow(LevelOpsMonitoringPeriodicWork.java:63)
	at io.levelops.plugins.jenkins.extensions.LevelOpsMonitoringPeriodicWork.execute(LevelOpsMonitoringPeriodicWork.java:51)
	at hudson.model.AsyncPeriodicWork.lambda$doRun$0(AsyncPeriodicWork.java:100)
	at java.lang.Thread.run(Thread.java:748)

Jul 08, 2020 3:00:15 PM INFO hudson.model.AsyncPeriodicWork lambda$doRun$0
Finished LevelOps Monitoring Worker Thread. 1,017 ms"
                mvn install'''
                    }
                }
                stage ('tsPackageSaas') {
                    steps {
                        sh 'ls -alf'
                    }
                }
                stage ('veritasDataload') {
                    steps {
                        sh 'ls -l'
                    }
                }
            }
        }
    }
}
