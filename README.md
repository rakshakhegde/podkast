# Java/Kotlin Podcast Feed Parser
_Simpler library to read podcast feeds_

## Usage
__Read Feed__
	
### Java

```java
Podcast podcast = PodcastLoader.load(new URL("FEED URL"));
System.out.println("Title - " + podcast.getTitle());
```

### Kotlin

```kotlin
val podcast = PodcastLoader.load(URL("FEED URL"))
println("Title - ${podcast.title}")
```

__Get Episodes__

### Java

```java
Podcast podcast = PodcastLoader.load(new URL("FEED URL"));
List<Episode> episodes = podcast.getEpisodes();
for(Episode episode : episodes) {
    System.out.println("Episode Title - " + episode.getTitle());
}
```

### Kotlin

```java
val podcast = PodcastLoader.load(URL("FEED URL"))
val episodes = podcast.episodes
episodes.forEach {
    println("Episode Title - ${it.title}"
}
```

## Inspiration
[Podcast-Feed-Library](https://github.com/MarkusLewis/Podcast-Feed-Library) _Original implementation in Java_
