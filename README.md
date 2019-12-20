# git_publish

Issues with the format of .cpanel.yml file when trying to deploy cpanel git repository to directory.

https://stackoverflow.com/questions/52688981/issues-with-the-format-of-cpanel-yml-file-when-trying-to-deploy-cpanel-git-repo

Please remove all "# comments" if you are copying the example or it might not work

---
deployment:
      tasks:
        - export DEPLOYPATH=/home/<username>/public_html/<app_folder>
        - /bin/cp <file_name> $DEPLOYPATH #Copy specific file to destination from root
        - /bin/cp /<sub_folder>/<file_name> $DEPLOYPATH #copy specific file from source sub folder
        - /bin cp * $DEPLOYPATH #copy all from root 
        - /bin cp /<sub_folder>/* $DEPLOYPATH #copy all from sub folder root
        
        
        
