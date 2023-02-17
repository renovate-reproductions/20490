# forking-renovate-repro

Reproducer to show a discrepancy in behavior between renovate bot and forking renovate 
when pulling a docker image tag from `ghcr.io`. 

With Mend renovate, the dependencies are getting recognized:

<img width="929" alt="Screenshot 2023-02-17 at 4 33 45 PM" src="https://user-images.githubusercontent.com/66699525/219798201-f7bb5ea9-5989-4d94-ba41-47687624ea2a.png">

With Forking Renovate,  we see the "Dependency Lookup Warning" for the same renvoate.json config :

<img width="969" alt="Screenshot 2023-02-17 at 4 39 47 PM" src="https://user-images.githubusercontent.com/66699525/219798952-02ab87f0-5f68-4189-8489-38d515478d9f.png">

On the other hand, pulling an image from Docker Hub (ubuntu) works fine for both.
