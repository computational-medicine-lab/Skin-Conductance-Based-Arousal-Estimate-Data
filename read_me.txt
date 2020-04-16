Please cite the following papers,

The results has been obtained using the methods in the following paper:  

Wickramasuriya DS, Amin MR and Faghih RT (2019) Skin Conductance as a Viable Alternative for Closing the Deep Brain Stimulation Loop in Neuropsychiatric Disorders. 
Front. Neurosci. 13:780. doi: 10.3389/fnins.2019.00780

Please refer to the following paper if you are using the skin conductance data:

Birjandtalab, J., Cogan, D., Pouyan, M.B. and Nourani, M., 2016, October. 
A non-EEG biosignals dataset for assessment and visualization of neurological status. In 2016 IEEE International Workshop on Signal Processing Systems (SiPS) (pp. 110-114). IEEE.



%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

1) File Name: Deconvolution_on_Experimental_data.mat


	Description: File contains deconvolution results on a 3 min segment (corresponding to Figure 2 in the paper) and sparse recovery result on 15 min 40 second segment (corresponding to Figure 4)

	field "deconv_result_on_3min_segment" contains the following variables
	u: 				recovered neural stimuli or ANS activity (sampling Freq. 4 Hz)
	tau_r: 				rise time of a skin conductance response 
	tau_d: 				decay time of a skin conductance response
	y_segment:			phasic skin conductance segment used for deconvolution (sampling Freq. 2 Hz)
	y_reconstructed_segment:	reconstructed phasic skin conductance segment


	field "sparse_recovery_on_15min_40sec_segment" contains the following variables
	u: 				recovered neural stimuli or ANS activity     (sampling Freq. 4 Hz)
	y_segment:			phasic skin conductance segment used for deconvolution      (sampling Freq. 2 Hz)



	"starting_time_of_task" field denotes the indices of the EDA where different time started
	
	other variables include raw_EDA data, tonic, phasic component and subject ID.

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

2) File Name: Deconvolution_on_Simulated_data.mat

	field "deconv_result_on_3min_segment" contains the following variables
	u: 				recovered neural stimuli or ANS activity (sampling Freq. 4 Hz)
	tau_r: 				rise time of a skin conductance response 
	tau_d: 				decay time of a skin conductance response
	y_segment:			simulated phasic skin conductance segment used for deconvolution (sampling Freq. 2 Hz)
	y_reconstructed_segment:	reconstructed phasic skin conductance segment



%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

3) File Name: Arousal_Tracking_Results.mat

	

	field "arousal_Tracking_result" contains the following variables
	
	u: 			        neural stimuli for 15 min 40 second signal 
					(mini emotional stress+cognitive stress+relaxation+emotional stress)
					
	Fsu: 				sampling Frequency for u
	binary:				binned Binary Data
	binary_bin_size:		size of the bin
	binary_bin_size_unit:		unit for the bin size
	arousal_state_Z: 		estimated arousal state at jth bin
	lower_confidence_level_of_Z:	calculated lower confidence level for Z with 95% confidence interval
	upper_confidence_level_of_Z:	calculated upper confidence level for Z with 95% confidence interval
	probability_of_a_peak_p:	calculated probability (p) of occuring an skin conductance response at jth bin
	lower_confidence_level_of_p:	calculated lower confidence level for Z with 95% confidence interval
	upper_confidence_level_of_p:	calculated upper confidence level for Z with 95% confidence interval
	high_arousal_index:		high arousal index (HAI)
	
