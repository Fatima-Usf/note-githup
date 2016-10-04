public class Rectangle extends Geometrie {


    public Rectangle() {
    }

    public Rectangle(double x, double y) {
        this.longeur = x;
        this.largeur = y;

    }

    public double getLongeur() {
        return longeur;
    }

    public void setLongeur(double longeur) {
        this.longeur = longeur;
    }

    public double getLargeur() {
        return largeur;
    }

    public void setLargeur(double largeur) {
        this.largeur = largeur;
    }

    @Override
    double perimetre() {
        return this.getLargeur() + this.getLongeur();
    }

    @Override
    double surface() {
        return this.getLargeur() * this.getLongeur();
    }

    @Override
    public String toString() {
        return super.toString() + "\nlongeur = " + this.getLongeur() + "\nlargeur = " + this.getLargeur() + "\nPerimetre = " + this.perimetre() + "\nSurface = " + this.surface();
    }
}
