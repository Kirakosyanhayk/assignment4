# assignment4


function matrixProduct(mat1,mat2) {
    let Array = "";
     for ( let i = 0; i < mat1.length; i++) {
        
         for ( let j = 0; j < mat2[0].length; j++) {
             let sum=0;
             for ( let k=0; k < mat1[0].length; k++) {
                 sum+= mat1[i][k] * mat2[k][j]
             }
           Array += sum + " "
         }
         Array += "\n"
     }
     return Array;
 }
 
 const mat1=[[1,2],
             [3,4],]
 const mat2=[[5,6],[7,8],]
 
 let Result= matrixProduct(mat1,mat2)
 console.log(Result)





function sumOfMatrices(mat1 = [],mat2 = []){
    let sum = 0
    let array = ""
    for(let i = 0; i< mat1.length; i++){
        for(let j=0; j<mat1[0].lenght; j++){
            sum = mat1[i][j] + mat2[i][j]
            array+=sum + " "
        }
        array+= "\n"
    }
    return array
}
    let mat1 = [[1,2],[3,4]]
    let mat2 = [[-1,-1],[-1,-1]]
    let Result = sumOfMatrices(mat1, mat2)
    console.log(Result) ;



 
 function sumofeachrow(mat = []){
     const result = []
     for(let i = 0; i < mat.length; i++ ){
         let sum = 0
         for(let j=0; j < mat[i].length; j++){
             sum +=mat[i][j]
         }
         result.push(sum)
     }
 console.log(result);
 }
