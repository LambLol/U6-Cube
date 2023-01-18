# U6-Cube

class Cube {

    private int side;

    public Cube() {
        side = 1;
    }
    public Cube(int s){
        side = s;
        if (side < 1){
            System.out.println("A cube’s side length cannot be less than 1!");
            throw new IllegalArgumentException();
        }
    }

    public int getSide(){
        return(side);
    }
    public void setSide(int s){
        side = s;
        if (side < 1) {
            System.out.println("A cube’s side length cannot be less than 1!");
            throw new IllegalArgumentException();
        }
    }
    public int getSurfaceArea(){
        return (int) Math. pow(side, 2) * 6;
    }
    public int getVolume(){
        return((int) Math. pow(side, 3));
    }
    public String toString(){
        return ("Cube{side=" + side + "}");
    }
}
