---
title: Astrology with Python
date: 2022-12-14 22:53:25
tags: coding
---
According to the Time Wave Theory, time is not a linear, uniform flow, but rather a complex, self-similar pattern that repeats itself at different scales. McKenna believed that this pattern is related to the evolution of consciousness and the emergence of novelty in the universe

We will be using Python to generate a human design chart with the following libraries:

### Libraries used (Prerequisites)
* Astrology 
* IChing
* Kabbalah

We will use the following libraries to generate a comprehensive body chart using western and eastern astrologicism. 

```python3
def generate_human_design(birth_date, birth_time, birth_place):
  natal_chart = astrology.calculate_natal_chart(birth_date, birth_time, birth_place)

  trigrams = iching.calculate_trigrams(natal_chart)

  bodygraph = kabbalah.calculate_bodygraph(trigrams)

  return bodygraph
```

### Example usage
```python3
my_birth_date = "January 1, 1991"
my_birth_time = "12:00 PM"
my_birth_place = "New York, NY"

my_human_design = generate_human_design(my_birth_date, my_birth_time, my_birth_place)

print(my_human_design)
```