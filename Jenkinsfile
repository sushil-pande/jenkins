pipeline
{
    agent any
    stages
    {
        parallel
        {
            stage("A")
            {
                agent {label: "aws"}
                steps
                {
                    echo "========executing A========"
                }   
            }
            stage("C")
            {
                steps
                agent {label: "aws"}
                {
                    echo "====++++executing C++++===="
                }
            }
            stage("D")
            {
                agent {label: "aws"}
                steps
                {
                    echo "====++++executing D++++===="
                }
            }
        }   
    }
}
