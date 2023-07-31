# LYPAP

The .rds is the R object of the analysed zebrafish marrow single cell dataset using VarID. 
It contains all the info one needs, including clusters, UMAP coordinates, normalised and raw counts. 
In order to see the expression pattern of any gene, load the .rds file into R using the readRDS command. 
Simply replace "ENSDARG00000035326" by the Ensembl ID of the gene of interest (see http://www.ensembl.org/Danio_rerio/Info/Index).

Command lines:

library(RaceID)
sc_varid_all <- readRDS("sc_varid_all.rds")
plotexpmap(sc_varid_all,"ENSDARG00000035326",logsc=F, um=F)
