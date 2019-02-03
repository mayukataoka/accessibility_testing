# Accessibility testing

##  Test https://bitsofco.de/
### Config file

'''
{
  "defaults": {
    "hideElements": "#carbonads",
    "ignore": [ "notice", "warning" ]
  },
  "urls": [ "https://bitsofco.de" ]
}
'''

### Test execution
'''
$ pa11y-ci --threshold 10
Running Pa11y on 1 URLs:
 > https://bitsofco.de - 0 errors

✔ 1/1 URLs passed
'''
