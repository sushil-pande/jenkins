pipeline
{
    agent any
    stages
    {
        parallel
        {
            stage("A")
            {
                agent aws
                steps
                {
                    echo "========executing A========"
                }   
            }
            stage("B")
            {
                steps
                agent aws
                {
                    echo "====++++executing B++++===="
                }
            }
            stage("C")
            {
                agent aws
                steps
                {
                    echo "====++++executing C++++===="
                }
            }
        }   
    }
}
