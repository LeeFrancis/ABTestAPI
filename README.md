# ABTestAPI
Make sure mongo db is up and running

1. install slc

npm i strongloop -g

2. cd into dir and run 

slc arc

3. use ui to post this to /Experiments

    {
        "json" : {
            "op" : "seq",
            "seq" : [ 
                {
                    "op" : "set",
                    "var" : "search_component",
                    "value" : {
                        "choices" : [ 
                            "MedicalSearch", 
                            "AcademicSearch"
                        ],
                        "op" : "uniformChoice",
                        "unit" : {
                            "op" : "get",
                            "var" : "id"
                        }
                    }
                }
            ]
        },
        "experiment" : "SearchBox Experiment"
    }

4. top right -> click on the play icon and start the api.
