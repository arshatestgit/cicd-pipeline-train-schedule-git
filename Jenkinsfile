pipeline
{
  agent any
  stages
  {
    stage ('Build')
    {
      steps{ echo "going to automate a build"
      sh ./gradlew build --no-daemon
      archiveArtifacts artifacts: '/dist/train-schedule.zip'
    }
    }
  }
}
