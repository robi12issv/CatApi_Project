# ABOUT THIS PROJECT

I made this project using [TheCatApi](https://thecatapi.com) database and [documentation](https://developers.thecatapi.com/view-account/ylX4blBYT9FaoVd6OhvR?report=bOoHBz-8t). The Kanban board can be found in [Jira](https://robibejenar.atlassian.net/jira/software/c/projects/LI/boards/3). It was written in Python, using the PyCharm IDE. I used unittest library for running the tests.  
The project marks the initial phase of establishing a veterinary clinic database tailored to cat owners with kids and/or dogs, who aspire to foster harmonious living among all family members.

## PROJECT'S STRUCTURES

The project has 2 main folders:
- `api_requests` with files that contain the methods for the requests
- `tests` with files with tests for each file from the `api_requests` folder.  
Aditionally, the project has the `main` file with the variables. 

## PROJECT USE INSTRUCTIONS

For cloning the project, open your preferred IDE and in the terminal, enter the command `git clone` followed by the project link, like this: 
`git clone https://github.com/robi12issv/CatApi_Project.git`

The `test_api` file contains tests for the basic requests such as getting images, filtering by breed and voting an image.  
The `test_cats_for_client` file contains tests that allow the user to extract, filter and return the cats that are most suitable for dog owners and children. The important aspect of these tests is that they are made for people that have dogs or kids and require a parameter that specifies whom the search is made for.  
The code follows the following steps: 
- filters the cat breeds based on atributes that increase the compatibility between cat and dogs or kids and displays the name of the breed and the value of the atributes;
- searches for images with those specific breeds and displays the `image_id` and the `link`;
- uses the `image_id` to vote the picture;
- filter the best votes made by the user and displays the images with the best cats.
The final result shows the picture url and it's rating:

![Screenshot 2024-04-07 at 21 05 59](https://github.com/robi12issv/CatApi_Project/assets/160391019/958765a0-5e46-45a7-943d-ef3a5e1c6d3b)

To change the type of the client (dog owners or kids), in `test_cats_for_client` change `client` variable from `dog` to `kids`

![Screenshot 2024-04-07 at 21 20 50](https://github.com/robi12issv/CatApi_Project/assets/160391019/0693e9a7-e215-4e20-a619-60b544a9b11f)

The tests run successfully and the coverage report showed a 97% coverage. 

![Screenshot 2024-04-17 at 19 40 44](https://github.com/robi12issv/CatApi/assets/160391019/1c187473-747e-4be5-9f7b-17254d7d70a5)
