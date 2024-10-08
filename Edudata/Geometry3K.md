https://opendatalab.com/OpenDataLab/Geometry3K/explore/main
# Description
one directory contains one questions

## Image
![img_diagram 1](https://github.com/user-attachments/assets/d960cf8f-1e19-48fe-a93b-0be0a199a99c)

![img_diagram_point](https://github.com/user-attachments/assets/a4a03503-e080-44ec-bc1a-7172e4c7db01)

## data.json
| Field              | Annotation                                | Example                                        |
| ------------------ | ----------------------------------------- | ---------------------------------------------- |
| problem_text       | the problem of the questions              | Find m \\angle C.                              |
| choices            | the choice of the problem                 | "38.25",<br>"43.75",<br>"51",<br>"51.75"       |
| answer             | the answer to the questions               | D                                              |
| detailed_solution  | the detailed information of the questions |                                                |
| problem_type_graph | the graph of the image                    | "Circle",<br>    "Triangle"                    |
| problem_type_goal  | the goal of the problem                   | Angle                                          |
| source             | the source of the question                | textbook1_chapter_10.pdf                       |
| comment            | the comment of the problem                |                                                |
| id                 | the id of the question                    | 2101                                           |
| annot_id           | the id of the annnotation                 | Shibiao_2020-03-28_09_36_19                    |
| is_standard        | true or false                             | false                                          |
| compact_choices    | the compact choices of the problem        | "38.25",<br>"43.75",<br>"51",<br>"51.75"       |
| precise_value      | the precise value of the choices          | 38.25,<br>    43.75,<br>    51.0,<br>    51.75 |
| rough_value        | the rough value of the choices            | 38.25,<br>    43.75,<br>    51,<br>    51.75   |
| compact_text       | the compact text of the problem           | Find m \\angle C.                              |
| annotat_text       | the text of annotation                    | Find $m \\angle C$                             |
| unit               | the unit of the problem                   |                                                |
| img_width          | the width of the image                    | 487                                            |
| img_height         | the height of the image                   | 427                                            |
| data_type          | the type of the data(text,train,val)      | val                                            |
| date               | the date of the questions                 | Fri Sep 18 22:23:14 2020                       |
| system             | the system of the problem                 | linux                                          |
## logic_form.json
| Field                     | Annotation                           | Example                                                                                                                                                                                                                                                                                               |
| ------------------------- | ------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| text_logic_form           | the logic form of the text           | Find(MeasureOf(Angle(C)))                                                                                                                                                                                                                                                                             |
| dissolved_text_logic_form | the dissolved logic form of the text | Find(MeasureOf(Angle(C)))                                                                                                                                                                                                                                                                             |
| diagram_logic_form        | the diagram logic form               | "Equals(MeasureOf(Angle(D, C, E)), 5x-12)",<br>    "Equals(MeasureOf(Angle(D, E, C)), 3x)",<br>    "PointLiesOnLine(B, Line(E, C))",<br>    "PointLiesOnCircle(E, Circle(B, radius_2_0))",<br>    "PointLiesOnCircle(C, Circle(B, radius_2_0))",<br>    "PointLiesOnCircle(D, Circle(B, radius_2_0))" |
| line_instances            | the instance of the line             | "BC",<br>    "DC",<br>    "EB",<br>    "EC",<br>    "ED"                                                                                                                                                                                                                                              |
| point_positions           | the position of the point            | "B": [<br>      159.0,<br>      160.0<br>    ],<br>    "C": [<br>      27.0,<br>      244.0<br>    ],<br>    "D": [<br>      25.0,<br>      77.0<br>    ],<br>    "E": [<br>      293.0,<br>      76.0<br>    ]                                                                                       |
| circle_instances          | the instances of the circle          | B                                                                                                                                                                                                                                                                                                     |
