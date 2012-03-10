<!SLIDE green-title padding-bottom>

# Hypermedia APIs

<!SLIDE green-title padding-bottom>

# Hypermedia APIs

<h2>Hypermedia designs scale better, are more easily changed and promote decoupling
and encapsulation, with all the benefits those things bring. </h2>

<!SLIDE green-title padding-bottom>

# Hypermedia APIs

<h2>On the downside, 
it is not necessarily the most latency-tolerant design, and caches can get stale
if you're not careful. It may not be as efficient on an individual request level
as other designs.</h2>

<!SLIDE green-title padding-bottom li-spacer>
<style>
</style>
# Hypermedia APIs

1. Use HTTP Properly<sup>*</sup>
2. Use Hypermedia to guide clients through business processes

<!SLIDE green-title little-bullets>

# Why HTTP?

* Client-Server
* Stateless
* Caching
* Uniform Interface
  * identification of resources
  * representations
  * self-descriptive messages 
  * hypermedia as the engine of application state
* Layered System
* Code-on-demand

<!SLIDE green-title little-bullets>

# Why HTTP?

* <strike>Client-Server</strike>
* <strike>Stateless</strike>
* <strike>Caching</strike>
* <strike>Uniform Interface</strike>
  * <strike>identification of resources</strike>
  * <strike>representations</strike>
  * <strike>self-descriptive messages </strike>
  * **hypermedia as the engine of application state**
* <strike>Layered System</strike>
* <strike>Code-on-demand</strike>

<!SLIDE>

# <code>GET /photos/12/delete</code>
