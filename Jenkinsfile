pipeline
{
    agent
    {
        label "any"
    }
    stages
    {
        parallel
        {
            stage("A")
            {
                agent "aws"
                steps
                {
                    echo "========executing A========"
                }   
            }
            stage("C")
            {
                steps
                agent "aws"
                {
                    echo "====++++executing C++++===="
                }
            }
            stage("D")
            {
                label "aws"
                steps
                {
                    echo "====++++executing D++++===="
                }
            }
        }   
    }
}
