# Technical Sizing Sanity Check 01
> (We usually have an engineer ask this question)
> Your engineers gave you the same size estimate - 1 hour - for each of the following three tasks that need to be done.  Which task feels like it should not be one hour, and why?
>  * Task: Swap the order of two fields in a form.  Size Estimate: 1 hour.
>  * Task: Make the delete button show a confirmation before it actually deletes:  Size Estimate: 1 hour.
>  * Task: Make your paginated table be sortable by any of the columns. Size Estimate: 1 hour
>
> If they don't volunteer a why, drill into the why for each.


## Reason
### Hypothesis
> Check that they have a basic understanding of web technology.  

### Measure of Success/Failure 
1. They identify that sorting a paginated table will likely involve server side work that will increase the size of this project.
2. Ideally they talk through why each of the other items is a bit easier, but potentially even talk about some problems or scenarios in which those may not be small either.  In reality, just with testing perhaps all of these should be bigger than 1 hour.

## Core Competency Coverage
- [ ] Product Design
- [ ] Product Strategy
- [ ] Analytical
- [x] Technical

## Attributions
* First encountered something like this from the guys at Reverb.  I thought it was a good idea for a base level technical competance.  If they can't get this one and it is a web related position, that should raise flags.

## Additional Reading

