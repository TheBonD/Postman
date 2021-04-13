
endpoint: object_info_1
method: GET
request_params: 
   1) age (int)
   2) weight (int)
   3) name (str)
response: 
`{'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}`
	  
------

endpoint: object_info_2
method: GET
request_params: 
   1) age (int)
   2) salary (int)
   3) name (str)

response:
`{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }`

------

endpoint: object_info_3
method: GET
request_params: 
   1) age (int)
   2) salary (int)
   3) name (str)

response: `
result = {'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'pets': {'cat':{'name':'Sunny',
                                     'age': 3},
                              'dog':{'name':'Luky',
                                     'age': 4}},
                     'u_salary_1_5_year': salary * 4}
          }`

------

endpoint: object_info_4
method: GET
request_params: 
   1) age (int)
   2) name (str)
   3) salary (int)

`response: 
result = {'name': name,
          'age': int(age),
          'salary': [salary, str(salary * 2), str(salary * 3)]}`

------

endpoint: user_info_1
method: POST
form_params: 
   1) age (int)
   2) weight (int)
   3) name (str)
   
response:`
{'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}
	  `
------

endpoint: user_info_2
method: POST
form_params: 
   1) age (int)
   2) salary (int)
   3) name (str)

response: `
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }`

------
endpoint: user_info_3
method: POST
form_params: 
   1) age (int)
   2) salary (int)
   3) name (str)

response: `
result = {'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'u_salary_1_5_year': salary * 4}
          }
`
------

endpoint: user_info_4
method: POST
form_params: 
   1) age (int)
   2) name (str)
   3) salary (int)

response: `
result = {'name': name,
          'age': int(age),
          'salary': [salary, str(salary * 2.5), str(salary * 3.5)]}

`
//decision
	
```json
{
   "info":{
      "_postman_id":"39b3713e-a319-4a09-a9c3-1c1bc1aee730",
      "name":"Vadim_QA",
      "schema":"https://schema.getpostman.com/json/collection/v2.1.0/collection.json"
   },
   "item":[
      {
         "name":"5 lesson",
         "item":[
            {
               "name":"HomeWork",
               "item":[
                  {
                     "name":"GET",
                     "item":[
                        {
                           "name":"object_info_1",
                           "request":{
                              "method":"GET",
                              "header":[
                                 
                              ],
                              "url":{
                                 "raw":"http://116.203.27.46:5002/object_info_1?age=100&weight=323&name=Roman",
                                 "protocol":"http",
                                 "host":[
                                    "116",
                                    "203",
                                    "27",
                                    "46"
                                 ],
                                 "port":"5002",
                                 "path":[
                                    "object_info_1"
                                 ],
                                 "query":[
                                    {
                                       "key":"age",
                                       "value":"100"
                                    },
                                    {
                                       "key":"weight",
                                       "value":"323"
                                    },
                                    {
                                       "key":"name",
                                       "value":"Roman"
                                    }
                                 ]
                              }
                           },
                           "response":[
                              
                           ]
                        },
                        {
                           "name":"object_info_2",
                           "request":{
                              "method":"GET",
                              "header":[
                                 
                              ],
                              "url":{
                                 "raw":"http://116.203.27.46:5002/object_info_2?age=26&salary=300&name=Roman",
                                 "protocol":"http",
                                 "host":[
                                    "116",
                                    "203",
                                    "27",
                                    "46"
                                 ],
                                 "port":"5002",
                                 "path":[
                                    "object_info_2"
                                 ],
                                 "query":[
                                    {
                                       "key":"age",
                                       "value":"26"
                                    },
                                    {
                                       "key":"salary",
                                       "value":"300"
                                    },
                                    {
                                       "key":"name",
                                       "value":"Roman"
                                    }
                                 ]
                              }
                           },
                           "response":[
                              
                           ]
                        },
                        {
                           "name":"object_info_3",
                           "request":{
                              "method":"GET",
                              "header":[
                                 
                              ],
                              "url":{
                                 "raw":"http://116.203.27.46:5002/object_info_3?age=100&salary=1500&name=Roman",
                                 "protocol":"http",
                                 "host":[
                                    "116",
                                    "203",
                                    "27",
                                    "46"
                                 ],
                                 "port":"5002",
                                 "path":[
                                    "object_info_3"
                                 ],
                                 "query":[
                                    {
                                       "key":"age",
                                       "value":"100"
                                    },
                                    {
                                       "key":"salary",
                                       "value":"1500"
                                    },
                                    {
                                       "key":"name",
                                       "value":"Roman"
                                    }
                                 ]
                              }
                           },
                           "response":[
                              
                           ]
                        },
                        {
                           "name":"object_info_4",
                           "request":{
                              "method":"GET",
                              "header":[
                                 
                              ],
                              "url":{
                                 "raw":"http://116.203.27.46:5002/object_info_4?name=Roman&age=20&salary=1000",
                                 "protocol":"http",
                                 "host":[
                                    "116",
                                    "203",
                                    "27",
                                    "46"
                                 ],
                                 "port":"5002",
                                 "path":[
                                    "object_info_4"
                                 ],
                                 "query":[
                                    {
                                       "key":"name",
                                       "value":"Roman"
                                    },
                                    {
                                       "key":"age",
                                       "value":"20"
                                    },
                                    {
                                       "key":"salary",
                                       "value":"1000"
                                    }
                                 ]
                              }
                           },
                           "response":[
                              
                           ]
                        }
                     ]
                  },
                  {
                     "name":"POST",
                     "item":[
                        {
                           "name":"user_info_1",
                           "request":{
                              "method":"POST",
                              "header":[
                                 
                              ],
                              "body":{
                                 "mode":"formdata",
                                 "formdata":[
                                    {
                                       "key":"age",
                                       "value":"20",
                                       "type":"text"
                                    },
                                    {
                                       "key":"weight",
                                       "value":"20",
                                       "type":"text"
                                    },
                                    {
                                       "key":"name",
                                       "value":"ROman",
                                       "type":"text"
                                    }
                                 ]
                              },
                              "url":{
                                 "raw":"http://116.203.27.46:5002/user_info_1",
                                 "protocol":"http",
                                 "host":[
                                    "116",
                                    "203",
                                    "27",
                                    "46"
                                 ],
                                 "port":"5002",
                                 "path":[
                                    "user_info_1"
                                 ]
                              }
                           },
                           "response":[
                              
                           ]
                        },
                        {
                           "name":"user_info_2",
                           "request":{
                              "method":"POST",
                              "header":[
                                 
                              ],
                              "body":{
                                 "mode":"formdata",
                                 "formdata":[
                                    {
                                       "key":"age",
                                       "value":"20",
                                       "type":"text"
                                    },
                                    {
                                       "key":"salary",
                                       "value":"400",
                                       "type":"text"
                                    },
                                    {
                                       "key":"name",
                                       "value":"ROman",
                                       "type":"text"
                                    }
                                 ]
                              },
                              "url":{
                                 "raw":"http://116.203.27.46:5002/user_info_2",
                                 "protocol":"http",
                                 "host":[
                                    "116",
                                    "203",
                                    "27",
                                    "46"
                                 ],
                                 "port":"5002",
                                 "path":[
                                    "user_info_2"
                                 ]
                              }
                           },
                           "response":[
                              
                           ]
                        },
                        {
                           "name":"user_info_3",
                           "request":{
                              "method":"POST",
                              "header":[
                                 
                              ],
                              "body":{
                                 "mode":"formdata",
                                 "formdata":[
                                    {
                                       "key":"age",
                                       "value":"20",
                                       "type":"text"
                                    },
                                    {
                                       "key":"salary",
                                       "value":"400",
                                       "type":"text"
                                    },
                                    {
                                       "key":"name",
                                       "value":"ROman",
                                       "type":"text"
                                    }
                                 ]
                              },
                              "url":{
                                 "raw":"http://116.203.27.46:5002/user_info_3",
                                 "protocol":"http",
                                 "host":[
                                    "116",
                                    "203",
                                    "27",
                                    "46"
                                 ],
                                 "port":"5002",
                                 "path":[
                                    "user_info_3"
                                 ]
                              }
                           },
                           "response":[
                              
                           ]
                        },
                        {
                           "name":"user_info_4",
                           "request":{
                              "method":"POST",
                              "header":[
                                 
                              ],
                              "body":{
                                 "mode":"formdata",
                                 "formdata":[
                                    {
                                       "key":"age",
                                       "value":"20",
                                       "type":"text"
                                    },
                                    {
                                       "key":"name",
                                       "value":"ROman",
                                       "type":"text"
                                    },
                                    {
                                       "key":"salary",
                                       "value":"500",
                                       "type":"text"
                                    }
                                 ]
                              },
                              "url":{
                                 "raw":"http://116.203.27.46:5002/user_info_4",
                                 "protocol":"http",
                                 "host":[
                                    "116",
                                    "203",
                                    "27",
                                    "46"
                                 ],
                                 "port":"5002",
                                 "path":[
                                    "user_info_4"
                                 ]
                              }
                           },
                           "response":[
                              
                           ]
                        }
                     ]
                  }
               ]
            },
            {
               "name":"FIRST",
               "request":{
                  "method":"GET",
                  "header":[
                     
                  ],
                  "url":{
                     "raw":"http://116.203.27.46:5002/first",
                     "protocol":"http",
                     "host":[
                        "116",
                        "203",
                        "27",
                        "46"
                     ],
                     "port":"5002",
                     "path":[
                        "first"
                     ]
                  }
               },
               "response":[
                  
               ]
            },
            {
               "name":"get.method",
               "event":[
                  {
                     "listen":"prerequest",
                     "script":{
                        "exec":[
                           ""
                        ],
                        "type":"text/javascript"
                     }
                  },
                  {
                     "listen":"test",
                     "script":{
                        "exec":[
                           "pm.test(\"Status code is 200\", function () {\r",
                           "    pm.response.to.have.status(200);\r",
                           "});"
                        ],
                        "type":"text/javascript"
                     }
                  }
               ],
               "protocolProfileBehavior":{
                  "disableBodyPruning":true
               },
               "request":{
                  "method":"GET",
                  "header":[
                     
                  ],
                  "body":{
                     "mode":"formdata",
                     "formdata":[
                        
                     ]
                  },
                  "url":{
                     "raw":"http://116.203.27.46:5002/get_method?name=Roman&age=500",
                     "protocol":"http",
                     "host":[
                        "116",
                        "203",
                        "27",
                        "46"
                     ],
                     "port":"5002",
                     "path":[
                        "get_method"
                     ],
                     "query":[
                        {
                           "key":"name",
                           "value":"Roman"
                        },
                        {
                           "key":"age",
                           "value":"500"
                        }
                     ]
                  }
               },
               "response":[
                  
               ]
            },
            {
               "name":"age_europe",
               "event":[
                  {
                     "listen":"test",
                     "script":{
                        "exec":[
                           "pm.test(\"Status code is 200\", function () {\r",
                           "    pm.response.to.have.status(200);\r",
                           "});"
                        ],
                        "type":"text/javascript"
                     }
                  }
               ],
               "request":{
                  "method":"POST",
                  "header":[
                     
                  ],
                  "body":{
                     "mode":"formdata",
                     "formdata":[
                        {
                           "key":"age",
                           "value":"99",
                           "type":"text"
                        }
                     ]
                  },
                  "url":{
                     "raw":"http://116.203.27.46:5002/age_europe?=",
                     "protocol":"http",
                     "host":[
                        "116",
                        "203",
                        "27",
                        "46"
                     ],
                     "port":"5002",
                     "path":[
                        "age_europe"
                     ],
                     "query":[
                        {
                           "key":"",
                           "value":""
                        }
                     ]
                  }
               },
               "response":[
                  
               ]
            }
         ]
      },
      {

```
