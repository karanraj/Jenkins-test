job('child1') {
  description("This is made by seedjob1 automation")
  /*scm {
	// fro adding github repo
		github(ownerAndProject='karanraj/Jenkins-test',branch='master')
    }*/
  triggers {
    
    	// for adding trigger periodically
        cron {
			spec(value='* * * * *')
		}
        // for adding pollscm trigger
        pollSCM {
			scmpoll_spec('* * * * *')
			// Ignore changes notified by SCM post-commit hooks.
			ignorePostCommitHooks(value=false)
		}
        //Github hook trigger
        gitHubPushTrigger()
   }

}
