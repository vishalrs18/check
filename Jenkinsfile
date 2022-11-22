import jenkins.model.Jenkins
node ('master') {
    stage("testing")
    {
        def job=Jenkins.instance
        def name=job.getJob("${target}")
        def build=name.scheduleBuild2(0)
        build.get()
    }
}
