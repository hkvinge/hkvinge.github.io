---
layout: post
title:  "A toy example: an LSTM learns Bach"
date:   2019-03-15 10:00:00 -0700
categories: jekyll update
---

Over the last few weeks I have been learning about LSTM networks. These are a family of recurrent neural networks that are useful for various learning tasks involving time series. We would like to use these networks in some of the work we have been doing on healthcare telemetry data and its relationship to variation in immune response. But as a fun project to get a better understanding of this tool, I wrote code to train an LSTM on midi files of Bach's chorales (I believe the LSTM trained on approximately 200). I was particularly interesting in what the behavior of a trained network would be if it were allowed to predict off its previous prediction for many time steps. As the networks made errors, would it wander off and get stuck in a fixed point or would it head off to output that did not sound like music?

You can listen [listen](https://soundcloud.com/user-105394224/an-lstm-wanders-off-on-a-bach) to an instance of the above situation. Surprisingly, the network continues to generate reasonable (though certainly not great) output. It is a still a little rough (you can hear many positions where the LSTM misses a note) but I intend to continue to refine the model to get something interesting.

The code for pre and post-processing the data for this project used [Music21](https://web.mit.edu/music21/). Additional functionality was written by [Manuchehr Aminian](https://www.math.colostate.edu/~aminian/). 
