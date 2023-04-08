README

## Directory Structure
.
├── README.txt
├── data
    ├── dev.a
    ├── dev.e
    ├── dev.f
├── output
    ├── best_guess_output.txt
    ├── best_guess_raw_alignments.txt
    ├── threshold_50_output.txt
├── a5.ipynb
├── a5.pdf
└── my_align


## Version
Python: 3.8.10


## Runtime
Algo 2 runs in 70s-80s per epoch on my laptop, and I found little improvement in my sample word probability after 8 epochs,
	which puts runtime around 10min total. 

## Notes:
Algo 1 and Algo 2 were developed and run primarily in the a5.ipynb notebook, but Algo 2 was converted into my_align in order
	to facilitate running via pipeline with check_alignments and score_alignments
I couldn't figure out how to install any of the off-the-shelf aligners linked in the assignment page, since they were all C++/Java,
	so I guess I'm leaving that out of the comparison in part 4.

## Results (also in Jupyter notebook):

Baseline output (-t 0.5):
Precision = 0.243110
Recall = 0.544379
AER = 0.681684

IMB Model 1, Threshold -t 0.5 output:
Precision = 0.834483
Recall = 0.340237
AER = 0.511387

IMB Model 1, Best Guess output:
Precision = 0.574202
Recall = 0.730769
AER = 0.375826

谢谢, now have yourself a damn fine day!
	~ 乐维