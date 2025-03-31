using System;
using System.Linq;
using System.IO;
using System.Text;
using System.Collections;
using System.Collections.Generic;

class Player
{
    enum LanderParams
    {
        X,
        Y,
        HSpeed,
        VSpeed,
        Fuel,
        Rotate,
        Power
    }

    class Lander
    {
        public int X;
        public int Y;
        public int hSpeed;
        public int vSpeed;
        public int fuel;
        public int rotate;
        public int power;

        public Lander(int X, int Y, int hSpeed, int vSpeed, int fuel, int rotate, int power)
        {
            this.X = X;
            this.Y = Y;
            this.hSpeed = hSpeed;
            this.vSpeed = vSpeed;
            this.fuel = fuel;
            this.rotate = rotate;
            this.power = power;
        }

        public void SaveLander()
        {
            if (rotate != 0)
            {
                rotate = 0;
            }

            if (-40 < vSpeed & vSpeed <= -35)
            {
                power = 4;
            }else{
                power = 2 ;
            }
            Console.WriteLine(rotate + " " + power);
        }
    }

    static void Main(string[] args)
    {
        string[] inputs;
        int surfaceN = int.Parse(Console.ReadLine());

        for (int i = 0; i < surfaceN; i++)
        {
            inputs = Console.ReadLine().Split(' ');
            int landX = int.Parse(inputs[(int)LanderParams.X]);
            int landY = int.Parse(inputs[(int)LanderParams.Y]);
        }

        while (true)
        {
            inputs = Console.ReadLine().Split(' ');
            int X = int.Parse(inputs[(int)LanderParams.X]);
            int Y = int.Parse(inputs[(int)LanderParams.Y]);
            int hSpeed = int.Parse(inputs[(int)LanderParams.HSpeed]);
            int vSpeed = int.Parse(inputs[(int)LanderParams.VSpeed]);
            int fuel = int.Parse(inputs[(int)LanderParams.Fuel]);
            int rotate = int.Parse(inputs[(int)LanderParams.Rotate]);
            int power = int.Parse(inputs[(int)LanderParams.Power]);

            Lander lander = new Lander(X, Y, hSpeed, vSpeed, fuel, 0, 0);
            lander.SaveLander();
        }
    }
}
