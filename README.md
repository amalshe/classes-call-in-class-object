# classes-call-in-class-object
void main() {
  First first = First(
      f1: 23,
      f2: Fourth(f1: 1, f2:(Seventh(se1:Sixth(si1: 544,si2: 3433,si3:Third(t1: 1112,t2: 23433,t3: 5678)) ,se2: 'aima',se3: 56)), f3: 4),
      f3: Third(
        t1: 5,
        t2: 6,
        t3: 7,
      ),
      f4: Second(s1: (Third(t1: 34, t2: 23, t3: 45)), s2: 9, s3: 10));
  Second second = Second(s1: Third(t1: 3, t2: 76, t3: 12), s2: 2, s3: 3);
  Third third =Third(t1:8,t2:9,t3:10);
  Fourth  forth =Fourth(f1:12,f2:(Seventh(se1: Sixth(si1: 1111,si2: 343,si3: Third(t1: 132,t2: 121,t3: 345)),se2: 'hira',se3:34)));
  Fifth fifth =Fifth(fi1: (Second(s1: Third(t1: 22,t2: 44,t3: 55), s2:344 , s3: 89)));
  Sixth sixth = Sixth(si1: 111,si2: 121,si3: Third(t1: 232,t2: 345,t3: 654));
  Seventh seventh = Seventh(se1:Sixth(si1: 234,si2: 34554,si3: Third(t1: 564,t2: 453,t3: 5677)),se2: 'acd',se3: 123 );
  Eighth eighth = Eighth(e1:First(f1: 1211,
      f2:Fourth(f1: 233,
          f2: Seventh(se1: Sixth(si1:  123,si2: 1233,
              si3: Third(t1: 233,t2: 4544,t3: 765)),
              se2: 'ghj',se3: 234)
          ,f3:12),f4: Second(s1: Third(t1: 122,t2: 432,t3: 656), s2: 124, s3: 432)));
  Ninth ninth= Ninth(n1:12,n2: 'asdf',n3: 344 );
  Tenth tenth= Tenth(te1: 432,te2: First(f1: 21,f2: Fourth(f1: 23,f2: Seventh(se1: Sixth(si1: 1234,si2: 1342,si3: Third(t1: 45,t2: 322,t3: 1244)),se2: 'sder',se3: 456))),te3: 9879);
}

class First {
  First({int f1 = 0, Fourth? f2, Third? f3, Second? f4}) {}
}

class Second {
  Second({required Third s1, required int s2, required int s3}) {}
}

class Third {
  Third({int t1 = 0, int t2 = 0, int t3 = 0}) {}
}

class Fourth {
  Fourth({int f1 = 0, Seventh? f2 , int f3 = 0}) {}
}

class Fifth {
  Fifth({Second? fi1 , String fi2 = 'amal', int fi3 = 0}) {}
}

class Sixth {
  Sixth({int si1 = 0, int si2 = 0, Third? si3}) {}
}

class Seventh {
  Seventh({Sixth? se1, String se2 = 'irha', int se3 = 0}) {}
}

class Eighth {
  Eighth({First? e1 , String e2 = 'huda', int e3 = 0}) {}
}

class Ninth {
  Ninth({int n1 = 0, String n2 = 'haya', int n3 = 0}) {}
}

class Tenth {
  Tenth({int te1 = 0, First? te2, int te3 = 0}) {}
}
