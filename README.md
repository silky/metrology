# Metrology

A library to easily measure what's going on in your python.

### Installing

To install :

    pip install metrology

## API

### Counters

    >>> from metrology import Metrology
    >>> counter = Metrology.counter('call')
    >>> counter.increment()

### Meters

    >>> from metrology import Metrology
    >>> meter = Metrology.meter('request')
    >>> meter.mark()

### Timers

    >>> from metrology import Metrology
    >>> timer = Metrology.timer('request')
    >>> with timer:
    ...     do()

### Utilization Timer

    >>> from metrology import Metrology
    >>> meter = Metrology.utilization_timer('request')    

## Reporters

### Logger Reporter

### Graphite Reporter

### Librato Reporter