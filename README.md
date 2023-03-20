# Calibration-recessions
# We are interested in modeling the NBER business cycle dating committee's procedure to determine when the economy is in a recession using a linear state space model. We define $x_t$ as the unobservable state of the economy and $r_t$ as the recession indicator, where
# rt = 1 [X_t <R]
# We make a strong assumption that the true data-generating process for $r_t$ features a linear time-invariant threshold. We later show empirically that this is a sensible assumption. 
# Our goal is to best fit the NBER's recession announcements $r_t$ observable from NBER data. To do so, we first consider different covariate specifications for the measurement vector $y_t$. Then, we search for a parameter calibration and linear threshold $R$ that defines our recession indicator estimated recession parameter $\hat{r}_t$. 

# We also consider the case in which $x_t = r_t$ in a subsequent section. 
# We define our model with the following linear state space set-up:
# xt+1 = ρxt + σwt+1 (state equation)
# yt = Gxt + νt (measurement equation)
# x0 ∼ N (μ0, Σ0)
# wt+1 ∼ N (0, 1)
# νt ∼ N (0, V )
# where for a given t = 0, 1, 2, ..., T , xt ∈ R is the unobservable state of the economy, yt ∈ Rm is a vector of observables used to characterize the state, ρ ∈ R is the persistence of the state’s transition dynamics, σ ∈ R is the volatility of noise in the state equation, G ∈ Rm is the output matrix, wt is noise.


