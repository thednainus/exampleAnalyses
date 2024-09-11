#' Get metadata of tip to use as deme in the phydynR model
#'
#' @param tip_name character
#'
#' @return character with the deme name that can be "I", "Tr", or "src". "I"
#'    corresponds to infected individuals; Tr corresponds to individuals
#'    on treatment and "src" corresponds to source sequences that account for
#'    importation in the phylodynamic analysis.
#' @export
get_metadata <- function(tip_name){

  #origin will be region or source
  origin <- str_split(tip_name, "_")[[1]]

  if(origin[2] == "src"){
    deme <- "src"
  }

  if(origin[2] == "region"){

    #care <- str_split(origin[3], "\\.")[[1]][3]

    #if(care == "care3"){
    #  deme <- "Tr"
    #}else{
    #  deme <- "I"
    #}
    deme <- "I"

  }

  return(deme)
}
