In an idea, tried to consider the SEM (stretched exponential method) as the correct forward model, but instead, Aprs model has been used inside EnKF algorithm to update the prior.
Then mismatch between Arps(ensemble) and SEM(ensemble) was calculated, and they were plotted as a function of the Aprs rate. The mean and standard devation of the mismatch has been computed with a sliding window.
And finally, with the first and second moments of data (mismatch), a normal random value has been generated and added to prior in EnkF update in each iteration.

Calculating RMSE of prior and posterior with and without adding model error showed some improvement. The updated result was closer to the updated proit when SEM was used as a forward model.


