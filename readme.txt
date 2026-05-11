data associated with paper:

Lackie, R., de Miranda, A.S., Lim, M.P., Novikov, V., Madner, N, Karunatilleke, N.C., Rutledge, B.S., Tullo, S., … Prado, M.A.M. (In preparation).
Stress-inducible phosphoprotein 1 (HOP/STI1/STIP1) regulates the spreading, aggregation, and toxicity of α-synuclein in vivo.

files:

prado_MRI_M83dTPR_subjectlist_final.csv is the demographics csv; includes all subjects included in the MRI analysis.
as mentioned in this csv, the files ending in: 
	1) *lsq6.mnc are the pre-processed subject images
		pre-processing consisted of 
			conversion from native Bruker to  NIfTI format (Neuroimaging Informatics Technology Initiative) to  MINC (Medical Imaging NetCDF) file format 
			image processing was performed using the MINC suite of software tools (http://bic-mni.github.io)
			the images were stripped of their native coordinate system, left-right flipped to compensate for Bruker’s native radiological coordinate system, denoised using patch-based adaptive non-local means algorithm (Coupe et al., 2008), and affinely registered to an average mouse template (the Dorr–Steadman–Ullman-Richards-Qiu-Egan atlas) to produce a rough brain mask
			a bias field correction was performed, and intensity inhomogeneity was corrected using N4ITK (Tustison et al., 2010) at a minimum distance of 5 mm
	2) *voted.mnc are the outputs of MAGeT-Brain segmentation pipeline (Chakravarty et al., 2013) using a modified/merged version of the Allen brain atlas (Lein et al., 2007)

Allen_brain_mapping_final.csv is a full list of the anatomical regions segmented in the modified Allen brain atlas

DSURQE_40micron_labels.mnc is the modified allen brain atlas labels on top of the Dorr–Steadman–Ullman-Richards-Qiu-Egan average mouse template (DSURQE_40micron.mnc)

