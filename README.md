# Dataset

The data used in the paper “A Two-Stage Approach for Two-Dimensional Bin Packing Problems Involving Rectangular and Irregular Shapes with Parts Priority” is provided here. The data is in JSON format, and the file names correspond to the case names in the paper. The specific details of each case are as follows:

“items”: information of parts.
"BackFrontPriority": indicating if a part is of priority. True represents a priority part; False represents an ordinary one.
"centPt": the center point of a part.
"id": id of a part.
"points": Coordinates of vertex of parts.
*"smallItem": inicating whether a part is in small size.
"plates": information of boards.
"height": the height of boards.
"width": the number of boards.
*"id": id of boards, is not used in the single bin size problem in this paper.
"number"： number of boards, in this research, it is unlimited, therefore set 9999.
*"surplus": indicating whether it is a surplus sheet, will be used in future research.
"prameters": prameters of the calculation.
*"remnantsSet"：difining remnant.
*"surplusDir": indicating whether the calculation create remnants.
"timeLimit": calculation time.


The elements marked with * were not used in the paper “A Two-Stage Approach for Two-Dimensional Bin Packing Problems Involving Rectangular and Irregular Shapes with Parts Priority”， but will be utilized in future research.
