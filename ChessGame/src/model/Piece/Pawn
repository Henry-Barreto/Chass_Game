@Override
public List getPossibleMoves() {
List moves = new ArrayList<>();
int direction = isWhite ? -1 : 1;
// Movimento para frente
Position front = new Position(
position.getRow() + direction,
position.getColumn()
);
if (front.isValid() && board.isPositionEmpty(front)) {
moves.add(front);
// Movimento duplo na primeira jogada
if ((isWhite && position.getRow() == 6) ||
(!isWhite && position.getRow() == 1)) {
Position doubleFront = new Position(
position.getRow() + 2 * direction,
position.getColumn()
);
if (board.isPositionEmpty(doubleFront)) {
moves.add(doubleFront);
}
}
}
// Capturas nas diagonais
// ...
return moves;
}