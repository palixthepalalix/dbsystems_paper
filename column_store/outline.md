
BACKGROUND
- why it is important
- what in the newer hardware or hardware developments makes column store attractive
- vague discription of types of optimizations

- go over the systems
	- where does the performance difference come from in each system
	- use this to talk about hybrids and different usages of each of hte techniques

HARDWARE

COMPRESSION/DEALING W COMPRESSED DATA

UPDATING

MATERIALIZATION

COMPARE TO ROW STORE

CRACKING->moving freq accessed columns closer together

HYBRID TECHNOLOGIES

VECTORIZED PROCESSING


TECHNOLOGIES
	- materialization
	- vector processing
	- comporession and diff compression algs; operating on this compressed data
	- db operations: column operations vs row operations, joins, aggs, ect ect
	- indexes?

COMPARE TECHNOLOGIES

	sybase IQ
		- Nbit and tiered indexing used for increased compresion and fast batch loads
		- each page composed of cells of variable size that are packed tightly together
		- col store architecture supports variable number of cells per page and various page formats within a column
		- Lempel-ziv-welch compression algorithms
		- bitmaps used for secondary indexes
	vertica
	vectorwise
	kx systems
	monet db
	amazon redshift
	citus db