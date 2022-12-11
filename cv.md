![my_photo](/my_photo1.jpg width="200" height="100")
# Kalieva Gulnara

## Junior Frontend Developer

## Contact 

**Location:** Moscow, Russia

**Phone:** +7-925-170-35-27

**E-mail:** laurieloko21@gmail.com

**GitHub:** [Kalieva Gulnara](https://github.com/danormalnaya)


## Education

**Financial Manager**

Moscow State Industrial University

2008-2013


**Programmer**

School 42 (Moscow campus)

2020-2021


## About me

I have been working in the restaurant business for more than 10 years. Thanks to my perseverance and desire, I was promoted to director and there were three objects in the management.

Now I want to change my field of activity, and I have no doubt that my skills and the ability to think outside the box will be a good addition to my work. The old love of mathematics and complex logic problems helped in solving being a programmer.

I studied at school 42, studied for a year and wrote projects in C and C++. However, the direction of the backend is not as much interested as the opportunity to develop in the frontend. I like the combination of precision of lines, as in architecture, and the search for aesthetics in design, as in drawing.

I have no experience in commercial IT projects. But I'm sure he'll be here soon.

## Skills

* C, C++
* HTML/CSS
* MySQL
* Git, Terminal
* ProCreate, Figma
* English: B1

## Review code on C:
> Re-code the set of the lib function. Functions will need to present the same prototype and behaviors as the original.
```C
char	*ft_substr(char const *s, unsigned int start, size_t len)
{
	size_t		i;
	char		*newstr;
	size_t		slen;

	if (!s)
		return (NULL);
	if (start > ft_strlen(s))
		return (ft_strdup(""));
	slen = ft_strlen(s + start);
	if (slen < len)
		len = slen;
	newstr = malloc(len + 1);
	if (!newstr)
		return (NULL);
	i = 0;
	while (s[start + i] && i < len)
	{
		newstr[i] = s[start + i];
		i++;
	}
	newstr[i] = '\0';
	return (newstr);
}
```

## Review code on C++:
> There are two boxes, the first one is A1×B1×C1, the second one is A2×B2×C2. Determine whether it is possible to place one of these boxes inside the other, provided that the boxes can only be rotated 90 degrees around the edges.
```C++
using namespace std;
int main()
{
    int a1, b1, c1, a2, b2, c2;
    std::cin >> a1 >> b1 >> c1 >> a2 >> b2 >> c2;
    int min1 = min(a1,min(b1,c1));
    int max1 = max(a1,max(b1,c1));
    int mid1 = (a1 + b1 + c1) - min1 - max1;
    int min2 = min(a2,min(b2,c2));
    int max2 = max(a2,max(b2,c2));
    int mid2 = (a2 + b2 + c2) - min2 - max2;
    if (min1 == min2 && max1 == max2 && mid1 == mid2)
        std::cout << "Boxes are equal";
    else if (min1 >= min2 && max1 >= max2 && mid1 >= mid2)
        std::cout << "The first box is larger than the second one";
    else if (min1 <= min2 && max1 <= max2 &&  mid1 <= mid2)
        std::cout << "The first box is smaller than the second one";
    else
        std::cout << "Boxes are incomparable";
  return 0;
}
```