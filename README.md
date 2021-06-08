# spring-quiz-app

Taken from this qwiklab https://google.qwiklabs.com/catalog_lab/968

### Show app doesnt persist data in DB
0. `cd start && mvn spring-boot:run`
0. Launch web preview on 8080 and create a question
0. In the GCP Console, click **Navigation menu > Datastore > Entities** and notice there's no data

### Show app persists data
0. Show changes in `./test/src/main/java/com/google/training/appdev/services/gcp/datastore/QuestionService.java`
0. `cd ./test && ./prepare_environment.sh`
0. `mvn spring-boot:run`
0. Create a question
0. In the GCP Console, click **Navigation menu > Datastore > Entities** and notice the data is persisted