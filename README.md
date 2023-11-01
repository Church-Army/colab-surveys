## Hi Siobhan

This is the repository we'll be using for any analysis of the 2023 Co.Lab survey's that Elspeth's just closed.

### About this directory

Here's what you can find here:

* `/survey-responses` contains survey response data, both in it's initial (.csv) form and the tidy-data that's output from `R/01_read-survey-data.html`.
* `/additional-data` contains a single text file, which is just the body of an email that Phoebe sent to Elspeth. You'll need to tabluate that data into a format that R can read if you want to analyse differences between the sample (survey respondents) and the population (CA staff)
* `R/` is where all our processes should live. I've kicked us of with `01_...`, and advise that you enumerate any further processes (i.e .qmd files) and save them there. 

I normally use a `data` subdirectory for storing all the data that goes into and out of the processes in `R/`, but this time I've opted not to, hence `survey-responses/` being its own thing in the project root. Just thought I'd try something new. The upshot of that is 'feel free to add more subdirectories to this directory as you see fit' - we want to keep everything comprehensible and tidy.

Note that this repo uses my new favourite package `renv` for reproducible package use. That means you'll need to `renv::restore()` after you pull and `renv::checkout()` before you push. It's literally that simple. You might also find that you need to re-install packages you already have installed, so don't be alarmed if that happens. 

## TODO

You'll need to liase with Elspeth directly for clear expectations on what she would like you to do, but I imagine some of the preliminary steps might be:

* Create `02_cleaning-survey-data`
	* Probably more like `02_A_cleaning-digital-practises-data`, and so on for each survey. I'll leave it to your judgement.
* Tabularise the data from the text file in `additional-data` (do this in Excel and ideally save as a CSV?)
* Carry out some analysis that compares the samples to the population of CA staff - see Elspeth for clearer steer about detail etc.

Have a great week while I'm away. See you soon!
	