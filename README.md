# Simple docker-compose setup for the Elastic Stack

This is a simple repository for spinning up a basic Elastic Stack environment that's suitable to begin a small project. No need to mess with java, ruby, dns, or fire wall! The data will be persisted on your disk, so you don't have to worry about recreating every time you spin this sucker up. See the docker-compose.yml file for more info

Running the following command will spin up Elasticsearch (:9200, :9300), Kibana (:5601), and Logstash

```bash
docker-compose up
```

So...what do you do next?

1. Import some data into Elasticsearch...maybe through the [Logstash](https://www.elastic.co/guide/en/logstash/current/getting-started-with-logstash.html)) config file (./logstash/logstash.conf)

2. Run a simple query through kibana by navigating to http://localhost:5601 and clicking on the "Dev Tools" tab.

Something like this ought to do!

```bash
GET /YOURINDEXNAMEHERE/_search
{ }
```

3. Not quire sure how to get started? Here are a couple of our ~biased~ favorite resources:

* [Coding Blocks Podcast on Search Engines](https://www.codingblocks.net/podcast/search-driven-apps/)
* [Search Engine Presentation, sample apps](https://github.com/codingblocks/search-driven-apps)

4. Still not quite got the hang of it? Reach out to [@codingblocks](https://twitter.com/codingblocks) on twitter and let us know what you're looking for and we'll get ya sorted!