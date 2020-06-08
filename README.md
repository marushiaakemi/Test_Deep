# Overview

The purpose of this task is to test your capabilities in developing algorithms to manipulate / convert the format of a dataset.

All you need to get started is python running on your machine!

# The Task

Oh no! We need to get an easy overview on some data of our internal project management tool, but the format of our database dump is a mess! Particularly, we would like to see what projects are under each of our managers and each of our watchers, in the right priority order. To explain these 2 user types (this doesn't have any impact on your task, just a side note):
- managers are the project managers with all grants for the projects they are managing and also get notifications for progress on those projects
- watchers have the same grants as managers, except that they don't get notifications. We need your help to get the data into a format that is easily readable!

<br/>
<br/>

The steps you should take:

* Download the source file: https://drive.google.com/file/d/1pJIynVU63BK9WGUSKPWTsHDCSPJG5hCb/view?usp=sharing. In the source json file you will encounter a list of dictionaries, each with the name of a project, the list of managers in that project, the list of watchers in the project and the priority interger of that project. **Very important here - the lower the interger, the higher the priority**
Example of one project's dictionary:
<br/>

```
{
        "name": "[CV] [Qt] OpenCV GUI",
        "managers": [
            "csaftoiu",
            "merlin"
        ],
        "watchers": [
            "merlin",
            "morris"
        ],
        "priority": 850
}
```
<br/>

* Generate 2 output files, watchers.json and managers.json. Each should contain a dictionary with the manager / watcher  in the key, and a list of projects in the value. The projects in the list should be ordered by priority - from highest to lowest (remember here that lower number means higher priority).
Example of one manager in the managers.json output file, in the correct format. The watchers.json file should follow the same format:

<br/>

```
"csaftoiu": [
        "sportsparsers - pinnacle API",
        "[OCR] tesseract MRZ reading ",
        "unity render diff passport text artur",
        "[CV] [Qt] OpenCV GUI",
        "unity render different passport text",
        "[template] unity render passport text",
        "matchbook parser - mfilho"
    ],
``` 
<br/>

Please commit both json files, and the code you used to generate them to a public github repository.

Good Luck!
