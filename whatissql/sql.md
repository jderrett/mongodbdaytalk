!SLIDE
# SQL vs. NoSQL

!SLIDE
# What is SQL?
## Structured.  Query.  Language.
### select * from wing_sauces
### i.e. "give me some data"

!SLIDE
# Set-based processing is cool
###Updates the first table based on joins to second table, i.e. "which wings need sauce"
	update wings a
	left join sauces b
	on a.sauce_id = b.id
	set a.needs_sauce = 1
	where b.id is null

!SLIDE
# Set-based processing is cool
###It can aggregate like a champ - "how many wings need sauce"
	select a.id, count(*)
	from wings a
	left join sauces b
	on a.sauce_id = b.id
	where b.id is null
	group by a.id


!SLIDE
# What is this NoSQL?
## Not very Structured.  Sort of Query.  Kind of Language.
### db.wing_sauces.find();
### i.e. "give me some data"

!SLIDE bullets incremental transition=blindY
# Can you use both?

* yes.
* (whew)
