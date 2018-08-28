# Use CAP Theorem to guide database choices when balancing consistency, availability, and partition-tolerance

 CAP (Consistency, Availability, and Partition Tolerance) theorem states that you can only guarantee two of the three CAP properties in a database system. In particular, this concept applies to distributed systems.

From [Wikipedia](https://en.wikipedia.org/wiki/CAP_theorem):
- Consistency: Every read receives the most recent write or an error
- Availability: Every request receives a (non-error) response – without guarantee that it contains the most recent write
- Partition tolerance: The system continues to operate despite an arbitrary number of messages being dropped (or delayed) by the network between nodes

> The decision between Consistency and Availability is a software trade off. You can choose what to do in the face of a network partition - the control is in your hands. Network outages, both temporary and permanent, are a fact of life and occur whether you want them to or not - this exists outside of your software.
>
>~ [Robert Greiner](http://robertgreiner.com/2014/08/cap-theorem-revisited/)


## Database Types and CAP
[Learning NoSQL Databases](https://www.lynda.com/NoSQL-tutorials/Up-Running-NoSQL-Databases/111598-2.html) suggests:
- SQL databases tend toward consistency and availability
- NoSQL solutions tend toward partition-tolerance

Depending on the size of the application, though, CAP may be irrelevant. 

See historical context of CAP Theorem in post by [Julian Browne](http://julianbrowne.com/article/brewers-cap-theorem).
