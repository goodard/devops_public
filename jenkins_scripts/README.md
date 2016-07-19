Install Jenkins jobs
=====================
1. Switch to jenkins OS user, then  copy $JOB_NAME/config.xml to /var/lib/jenkins/jobs/$JOB_NAME/config.xml

2. Restart Jenkins, or reload Jenkins configuration from GUI

Update Common Library Checksum 
==============================
```
cd /Users/mac/baidu/*/private_data/project/devops_consultant/consultant_code/devops_public/jenkins_scripts
find . -name "*.sh" | xargs sed  -i "" "s/2550329384/472987608/g"
find . -name "*.sh" | xargs grep "bash /var/lib/devops/refresh_common_library.sh"
```