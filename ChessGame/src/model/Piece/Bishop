@Override
public List getPossibleMoves() {
List moves = new ArrayList<>();
// Direções diagonais:
// superior-esquerda, superior-direita,
// inferior-esquerda, inferior-direita
int[][] directions = {
{-1, -1}, {-1, 1},
{1, -1}, {1, 1}
};
for (int[] direction : directions) {
int row = position.getRow();
int col = position.getColumn();
while (true) {
row += direction[0];
col += direction[1];
Position newPos = new Position(row, col);
if (!newPos.isValid()) break;
Piece pieceAt = board.getPieceAt(newPos);
if (pieceAt == null) {
moves.add(newPos);
} else if (pieceAt.isWhite() != isWhite) {
moves.add(newPos);
break;
} else {
break;
}
}
}
return moves;
}