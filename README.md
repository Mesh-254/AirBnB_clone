# 0x00. AirBnB clone - The console

Airbnb Clone is a technical solution to entrepreneurs for launching their own rental marketplace platform faster into the market. It is equipped with essential features to run a marketplace where customers can share their properties and also goods easily.

Command interpreter
=

. Create a new object (ex: a new User or a new Place)

. Retrieve an object from a file, a database etc…

. Do operations on objects (count, compute stats, etc…)

. Update attributes of an object

. Destroy an object

# Resources

. cmd module

. packages concept page

. uuid module

. datetime

. unittest module

. args/kwargs

Installation
=
.  Clone the repository. git clone https://git@github.com:MahiET/AirBnB_clone.git

.  Open the /AirBnB_clone directory and execute console.py

Setup

.  You need Python interpreter. IMPORTANT: The project was created in UBUNTU  20.04  LTS and Python 3.9

Interactive Mode

   (hbnb) help

      EOF  help  quit

        (hbnb) 

          (hbnb) 

           (hbnb) quit
    
          $

$ ./console.py
(hbnb) create BaseModel
5dccfbf9-03a6-45f7-8a75-80094392bf97
(hbnb) show BaseModel 5dccfbf9-03a6-45f7-8a75-80094392bf97
[BaseModel] (5dccfbf9-03a6-45f7-8a75-80094392bf97) {'id': '5dccfbf9-03a6-45f7-8a75-80094392bf97', 'updated_at': datetime.datetime(2018, 6, 13, 23, 10, 13, 549740), 'created_at': datetime.datetime(2018, 6, 13, 23, 10, 13, 549699)}
(hbnb) all
[[BaseModel] (5dccfbf9-03a6-45f7-8a75-80094392bf97) {'id': '5dccfbf9-03a6-45f7-8a75-80094392bf97', 'updated_at': datetime.datetime(2018, 6, 13, 23, 10, 13, 549740), 'created_at': datetime.datetime(2018, 6, 13, 23, 10, 13, 549699)}]
(hbnb) BaseModel.count
1
(hbnb) update BaseModel 5dccfbf9-03a6-45f7-8a75-80094392bf97 number 89
(hbnb) show BaseModel 5dccfbf9-03a6-45f7-8a75-80094392bf97
[BaseModel] (5dccfbf9-03a6-45f7-8a75-80094392bf97) {'number': '89', 'updated_at': datetime.datetime(2018, 6, 13, 23, 11, 51, 470426), 'created_at': datetime.datetime(2018, 6, 13, 23, 10, 13, 549699), 'id': '5dccfbf9-03a6-45f7-8a75-80094392bf97'}
(hbnb) create User
71e19890-6440-4ca9-9976-59ba61571f09
(hbnb) all
[[User] (71e19890-6440-4ca9-9976-59ba61571f09) {'id': '71e19890-6440-4ca9-9976-59ba61571f09', 'updated_at': datetime.datetime(2018, 6, 13, 23, 12, 39, 71568), 'created_at': datetime.datetime(2018, 6, 13, 23, 12, 39, 71532)}, [BaseModel] (5dccfbf9-03a6-45f7-8a75-80094392bf97) {'number': '89', 'updated_at': datetime.datetime(2018, 6, 13, 23, 11, 51, 470426), 'created_at': datetime.datetime(2018, 6, 13, 23, 10, 13, 549699), 'id': '5dccfbf9-03a6-45f7-8a75-80094392bf97'}]
(hbnb) destroy User 71e19890-6440-4ca9-9976-59ba61571f09
(hbnb) all
[[BaseModel] (5dccfbf9-03a6-45f7-8a75-80094392bf97) {'number': '89', 'updated_at': datetime.datetime(2018, 6, 13, 23, 11, 51, 470426), 'created_at': datetime.datetime(2018, 6, 13, 23, 10, 13, 549699), 'id': '5dccfbf9-03a6-45f7-8a75-80094392bf97'}]
(hbnb) destroy BaseModel 5dccfbf9-03a6-45f7-8a75-80094392bf97
(hbnb) all
[]
(hbnb) quit
$



Non-Interactive Mode

    (hbnb)

      EOF  help  quit

       (hbnb) 

        $

          $ cat test_help

           help

           $

            $ cat test_help | ./console.py

             (hbnb)

               EOF  help  quit

               (hbnb)

                  $


(hbnb) $
$

$ echo "create BaseModel" | ./console.py
(hbnb) 0b64b088-3e45-4ee7-a08e-37a0050a63e2
(hbnb) $

echo "all" | ./console.py
(hbnb) ["[BaseModel] (0f96a2b4-8376-4f60-8b7f-f124e5696e45) {'id': '0f96a2b4-8376-4f60-8b7f-f124e5696e45', 'created_at': datetime.datetime(2022, 1, 31, 5, 15, 9, 934710), 'updated_at': datetime.datetime(2022, 1, 31, 5, 15, 9, 935025)}", '[BaseModel] (8b88194a-fd2c-4825-a7dd-bd24f013fd7c) {\'id\': \'8b88194a-fd2c-4825-a7dd-bd24f013fd7c\', \'created_at\': datetime.datetime(2022, 1, 31, 5, 42, 20, 775402), \'updated_at\': datetime.datetime(2022, 1, 31, 5, 42, 20, 775732), \'first_name\': \'"Betty"\'}', "[BaseModel] (0b64b088-3e45-4ee7-a08e-37a0050a63e2) {'id': '0b64b088-3e45-4ee7-a08e-37a0050a63e2', 'created_at': datetime.datetime(2022, 1, 31, 5, 51, 0, 221529), 'updated_at': datetime.datetime(2022, 1, 31, 5, 51, 0, 221874)}", "[BaseModel] (6631236f-543a-4437-9b42-06a9877c1e6e) {'id': '6631236f-543a-4437-9b42-06a9877c1e6e', 'created_at': datetime.datetime(2022, 1, 31, 5, 52, 51, 671162), 'updated_at': datetime.datetime(2022, 1, 31, 5, 52, 51, 671494)}"]
(hbnb) $
$
	       

  Authors

Meaza Lemma - Meazalemma2020@gmail.com || MahiET

Meshack Mutune  @Mesh-254




      
