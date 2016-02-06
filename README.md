# community.zenoss.org archive

```
wget --mirror -p --html-extension --convert-links -e robots=off -P .  --domains community.zenoss.org http://community.zenoss.org/

# du -sh *
2.3G    community.zenoss.org

rm -rf community.zenoss.org/tags*
rm -rf community.zenoss.org/people*
find community.zenoss.org -name "*?decorator=print*" -exec rm {} \;
find community.zenoss.org -name "*?tstart=0.html*" -exec rm {} \;
find community.zenoss.org -name "*?view=tags&tags=*" -exec rm {} \;
find community.zenoss.org/message/ -name "[1-5]*.html" -exec rm {} \;
rm -rf community.zenoss.org/emailPasswordT* community.zenoss.org/forgot-username* community.zenoss.org/login* community.zenoss.org/opensearch.xml community.zenoss.org/blogs* community.zenoss.org/4* community.zenoss.org/polls*

# du -sh
882M    community.zenoss.org
```
